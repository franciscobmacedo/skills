---
name: tlim
description: Answer questions using the TLIM Boletim archive — David Almas's monthly Portuguese personal-finance newsletter (PPRs, ETFs, brokers, IRS, mortgages, Segurança Social, retirement). Use whenever the user asks what David Almas / TLIM says about a topic, or wants Portuguese personal-finance guidance grounded in the newsletter, e.g. "o que diz o David Almas sobre…", "check tlim", "search the boletim".
---

# TLIM Boletim archive

Monthly personal-finance newsletter by David Almas (Portuguese). One markdown
file per issue, with frontmatter (`title`, `date`, `uid`, `source`). New issues
land around the 1st of each month.

## Where the content lives

`https://tlim.fmacedo.com/md/index.md` is the table of contents (date + title
per issue); each entry links to `https://tlim.fmacedo.com/md/<file>.md`.

## How to answer a question

1. Fetch the index for the list of issues.
2. Pick the issues whose titles match the topic and fetch those files —
   searching works best with Portuguese terms.
3. Prefer the most relevant issue(s) over reading many; files are 40–500KB,
   and long data tables are flattened into `pre` blocks.
4. Cite the issue by title and date, and link `source:` (tlim.pt) or
   `https://tlim.fmacedo.com` so the user can open the original.

## Notes

- Content is in Portuguese; answer in the user's language.
- Almas's recommendations evolve — prefer the most recent issue on a topic, and
  say which edition a claim comes from.
- The newsletter is David Almas's paid work; quote sparingly, summarize instead.
