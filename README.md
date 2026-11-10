# skills

Agent skills by [@franciscobmacedo](https://github.com/franciscobmacedo), installable with the [skills CLI](https://skills.sh):

```bash
npx skills add franciscobmacedo/skills            # all skills
npx skills add franciscobmacedo/skills --skill conductor
```

## Skills

| Skill | What it does |
|---|---|
| [`conductor`](skills/conductor/SKILL.md) | Round-based orchestration for building products iteratively: one persistent worker agent in its own terminal pane, fed engineered briefs as the user reacts, monitored in the background, with outcomes (not logs) reported back. |
| [`founder`](skills/founder/SKILL.md) | Founder mode: the agent is the founder, CEO, CTO and CFO of a product and the user is only the investor. It validates the idea first, makes every decision, runs relentlessly with sub-agents inside one session, keeps its state in files, and contacts the user only for logins, real money, or a milestone to try. Builds on `conductor`. |
| [`tlim`](skills/tlim/SKILL.md) | Answer questions from the TLIM Boletim archive — David Almas's monthly Portuguese personal-finance newsletter (PPRs, ETFs, brokers, IRS, mortgages, retirement) at tlim.fmacedo.com. |
| [`portugues-de-portugal`](skills/portugues-de-portugal/SKILL.md) | Write natural, professional European Portuguese (Portugal): no Brazilian usage, no English calques, no em dashes, and plain reader-first writing for clients and public bodies. |

More to come.
