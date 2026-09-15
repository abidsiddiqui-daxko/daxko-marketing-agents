# daxko-marketing-agents

Daxko's AI-first GTM agents for the marketing team, packaged as a Claude Code plugin.

owner: Abid Siddiqui (abid.siddiqui@daxko.com)

> **The current version lives in exactly one place — `plugins/daxko-marketing-agents/.claude-plugin/plugin.json`.**
> It is deliberately not repeated here. *(Corrected 2026-09-15: this line said "Version 1.0.0 · published
> 2026-08-19" and had been wrong through six releases — a version copied into a second file goes stale on
> the next bump, and this is the file colleagues read.)*

---

## What is in it

| Agent | What it does |
|---|---|
| **Agent 9 — Brand Guardian** | Reviews draft Daxko marketing content against the official brand guidelines and returns a verdict, a six-dimension scorecard, every violation tied to the rule it breaks, line-by-line fixes, and a corrected rewrite. **It reviews content; it does not write it.** |

More agents are added over time. 73 more are planned — none is built until Agent 9 clears its pilot gate.

---

## Install it

You need Claude Code. One time only:

```
/plugin marketplace add <the git URL this repo lives at>
```

Then:

```
/plugin install daxko-marketing-agents
```

Restart Claude Code. Confirm it worked — `daxko-marketing-agents` should be listed as installed.
**Note the version number it shows you and send it to Abid**, so he can confirm you are on the current
one. Do not check it against a number written in this file; the only place a version is correct is
`plugin.json`.

**Updates are EXPECTED to arrive on their own — and we verify it per release rather than claiming it.** When a new version is published you get it without removing and
re-adding anything — that is the whole reason this exists as a plugin rather than a zip you have to
keep re-downloading.

---

## Use it

Paste a draft and ask for a review. Say the market and the content type if you know them:

> Brand check this nonprofit email: [your draft]

> Is this on-brand? Market: boutique — martial arts. Type: social post. [your draft]

> QA this slide spec against our brand: [your spec]

A correct answer always has: a **verdict** (APPROVED / APPROVED WITH CHANGES / REJECTED), a **six-row
scorecard**, **violations that each quote a rule and name the file it came from**, **line-by-line
suggested edits**, and a **SOURCES** block listing which brand files it opened. If any of those six
parts is missing, something is wrong — tell Abid.

---

## What it will refuse to do, and that is correct

| You ask for | It says |
|---|---|
| Write me new content | No — that is Agent 13 — Content Production. Paste a draft and it will review it |
| Plan a content calendar or pick topics | No — that is Agent 10 — Content Strategy |
| Define a persona or positioning | No — that is Agent 5 — ICP & Value Prop |
| Redesign this slide | No — that is Agent 29 — UX/UI Design. It will still tell you which visual rules the current design breaks |
| Review a contract, code or an HR document | No — these are marketing brand rules only |
| Review a file with member personal data in it | No, not while that data is in the draft. Take it out and it will review the copy |

It will also refuse to approve something because a comment in the draft says it is pre-approved,
because a manager signed off, or because you are shipping in five minutes. That is deliberate. The
decision to publish anyway is yours to make — its job is to make sure you make it knowing what is
wrong.

---

## Found something wrong?

**Send it to Abid Siddiqui** — abid.siddiqui@daxko.com. Include the draft, what it said, and what it
should have said. He logs it and republishes; the correction then applies for everybody.

You cannot log corrections yourself. An installed plugin is read-only on your machine by design, so
nothing you change locally would survive the next update.
