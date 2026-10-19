---
name: tlim
description: Answer questions using the TLIM Boletim archive — David Almas's monthly Portuguese personal-finance newsletter (PPRs, ETFs, brokers, IRS, mortgages, Segurança Social, retirement). Use whenever the user asks what David Almas / TLIM says about a topic, or wants Portuguese personal-finance guidance grounded in the newsletter, e.g. "o que diz o David Almas sobre…", "check tlim", "search the boletim".
---

# TLIM Boletim archive

Monthly personal-finance newsletter by David Almas (Portuguese). One markdown
file per issue, with frontmatter (`title`, `date`, `uid`, `source`). New issues
land around the 1st of each month.

## Retrieve and find evidence

- Start from `https://tlim.fmacedo.com/llms.txt`: short reading instructions
  plus every issue (newest first) with absolute links to its markdown file.
  `https://tlim.fmacedo.com/md/index.md` has the same list, oldest first. Check
  the latest available date and relevant gaps; this is an archive, not a
  guarantee of complete coverage.
- Do not scrape the homepage HTML or open a browser: the homepage builds its
  list with JavaScript. Everything needed is in `llms.txt`, `md/` and
  `search-index.json`.
- Yearly investment recommendations (funds, ISINs, exchanges, brokers) are in
  the 1 January issue of each year; read the latest one first for "what should
  I buy / which broker or exchange" questions.
- Titles describe only part of each issue. Search
  `https://tlim.fmacedo.com/search-index.json` for the topic, including Q&A hidden
  under unrelated titles. Its `articles` array contains `uid` and full `text`.
  Download and search locally using Portuguese terms, synonyms and phrases; return
  short surrounding excerpts, not the entire index. Map matching UIDs to the
  issue filenames in the markdown index. Broaden or refine terms when matches are
  absent or noisy; a missing title match does not establish missing coverage.
- Fetch the most relevant matching issues and read the surrounding passages.
  Check newer topic matches for changes to earlier recommendations. Distinguish a
  recommended purchase from a personal holding or a product merely under review.
- If a web tool cannot fetch these URLs, try `curl -fsSL` or Python's
  `urllib.request` before concluding the archive is unavailable. For example:

  ```sh
  curl -fsSL https://tlim.fmacedo.com/llms.txt
  curl -fsSL https://tlim.fmacedo.com/search-index.json -o /tmp/tlim-search.json
  ```

## Read large issues and calculators

Issues can be hundreds of kilobytes. Flattened tables in fenced code blocks or
`pre` elements can repeat large amounts of text. Use bounded excerpts for prose;
omit these blocks from a prose-only reading, and inspect them separately if the
question depends on their data. Avoid printing whole issues or giant matching
lines into context.

Some interactive calculators lose their inputs during conversion, concatenate
selectors, or expose placeholders such as `xx euros`. Do not use those outputs
as calculated results, even when an amount looks plausible. Link the original
interactive tool if available, or calculate independently from explicit,
verified inputs and label your assumptions. Do not guess missing table values.

## Answer and cite

- Answer in the user's language, summarizing rather than quoting extensively.
- Cite the issue title, date and relevant section using the **direct mirror
  markdown URL actually fetched**, not just the archive homepage. The frontmatter
  `source:` can be `None` or a dead original URL; use it only after checking that
  it opens the intended issue. A verified direct HTML mirror is also suitable.
- Separate Almas's dated statements from your application to the user's
  circumstances. If no direct answer is found, identify the limits of the search
  and label inference instead of attributing a personalized recommendation to him.
- Do not treat historical fees, rates, forecasts or tax statements as current.
  When the answer depends on current law or product terms, verify those with the
  tax authority, regulator or provider and cite them separately. Future rules or
  account eligibility cannot be promised from an old newsletter.
- For a personal investment choice, make material assumptions visible and obtain
  missing details such as horizon, liquidity needs, debts and risk tolerance
  before presenting a specific allocation as suitable. Describing the author's
  views does not require inventing a personal financial profile.
