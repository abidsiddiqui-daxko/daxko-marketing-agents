# daxko-marketing-agents

Daxko's AI-first GTM agents for the marketing team, packaged as a Claude Code plugin.

owner: Abid Siddiqui (abid.siddiqui@daxko.com)

> **The current version lives in exactly one place — `plugins/daxko-marketing-agents/.claude-plugin/plugin.json`.**
> It is deliberately not repeated here. *(Corrected 2026-09-15: this line said "Version 1.0.0 · published
> 2026-08-19" and had been wrong through six releases — a version copied into a second file goes stale on
> the next bump, and this is the file colleagues read.)*

---

## What is in it

**Agent name vs skill name.** Each agent has a name for people ("Agent 15 — Email & Nurture") and a short
skill name that Claude uses to pick it (`daxko-email-nurture`). Skill names can only use small letters,
numbers and hyphens, so the two never look the same. Use this table to match them.

**How to read this table:** one row per agent. *Skill #* counts the skills — Agents 63, 64 and 65 share
skill #12, which is why there are 21 rows but only 19 skills. *Ask it like this* is copied from the
skill's own description. *First published* is checked against the plugin repo's git history.
*Batch 1* skills are out with stakeholders for testing and are not changed; *Batch 2* skills are live.

| S.No | Skill # | Batch | Agent (number — name) | Skill name (what Claude calls it) | What it does, in plain words | Ask it like this | First published | Status today |
|---|---|---|---|---|---|---|---|---|
| 1 | 1 | 1 | Agent 2 — OKR Copilot | `daxko-okr-copilot` | Turns Daxko's goals (OKRs) into a quarter plan: what to do, in what order, by when. | "help me plan Q1" | v1.7.10 | Out for stakeholder testing |
| 2 | 2 | 1 | Agent 5 — ICP & Value Prop | `daxko-icp-value-prop` | Says who Daxko sells to and what to say to them, from approved buyer files. | "what is our ICP for JCCs" | v1.7.14 | Out for stakeholder testing |
| 3 | 3 | 1 | Agent 9 — Brand Guardian | `daxko-brand-guardian` | Checks a draft against Daxko's brand rules and gives fixes. Reviews only, never writes. | "is this on-brand" + paste the draft | v1.0.0 | Out for stakeholder testing |
| 4 | 4 | 1 | Agent 11 — Thought Leadership & Long-Form | `daxko-thought-leadership` | Writes one long piece: a whitepaper, eBook, research report or executive article. | "I need a research report on X" | v1.7.7 | Out for stakeholder testing |
| 5 | 5 | 1 | Agent 13 — Content Production | `daxko-content-production` | Writes a full set of matching pieces (email, social, page…) for one launch or campaign. | "all the assets for this launch" | v1.7.0 | Out for stakeholder testing |
| 6 | 6 | 1 | Agent 14 — Content Repurposing | `daxko-content-repurposing` | Turns one finished piece you paste into several new formats. | "repurpose this webinar transcript" | v1.7.15 | Out for stakeholder testing |
| 7 | 7 | 1 | Agent 18 — Marketing Performance | `daxko-marketing-performance` | Explains what marketing numbers you paste mean for a Daxko goal. | "how did Q3 go" | v1.7.6 | Out for stakeholder testing |
| 8 | 8 | 2 | Agent 3 — Market Intelligence & Competitive | `daxko-market-intelligence` | Answers questions about competitors and the market from Daxko's competitor files. | "where do we win and lose against Mindbody" | v1.7.22 | Live in claude.ai |
| 9 | 9 | 2 | Agent 67 — Customer Proof & Advocacy | `daxko-customer-proof` | Says which customer stories and quotes are approved, and drafts asks for reviews, quotes or case studies. | "draft a testimonial request" | v1.7.23 | Live in claude.ai |
| 10 | 10 | 2 | Agent 51 — Roadmap & Release Briefing | `daxko-release-briefing` | Turns release notes you paste into a short internal briefing: what changed and what we may say. | "brief the sales team on this release" | v1.7.24 | Live in claude.ai |
| 11 | 11 | 2 | Agent 50 — Product Insights & Feedback | `daxko-feedback-insights` | Finds the main themes in customer feedback you paste. | "make sense of these NPS comments" | v1.7.25 | Live in claude.ai |
| 12 | 12 | 2 | Agent 63 — Non-Profit Campaign & Content Strategist | `daxko-campaign-brief` (shared) | Plans a campaign and writes the brief for YMCAs, JCCs and Boys & Girls Clubs. | "plan a Q1 campaign for mid-size YMCAs" | v1.7.27 | Live in claude.ai |
| 13 | 12 | 2 | Agent 64 — Club Campaign & Content Strategist | `daxko-campaign-brief` (shared) | Same job for health clubs. | "campaign brief for clubs leaving ABC Fitness" | v1.7.27 | Live in claude.ai |
| 14 | 12 | 2 | Agent 65 — Boutique Campaign & Content Strategist | `daxko-campaign-brief` (shared) | Same job for martial arts and functional fitness. | "messaging for a BJJ studio switcher campaign" | v1.7.27 | Live in claude.ai |
| 15 | 13 | 2 | Agent 20 — Battlecard & Objection Handling | `daxko-battlecards` | Makes internal battle cards against a competitor, and ready answers when a buyer pushes back. | "battle card for Amilia" | v1.7.28 | Live in claude.ai |
| 16 | 14 | 2 | Agent 21 — Sales Enablement | `daxko-sales-kit` | Drafts sales materials: one-pager, deck outline, discovery questions, demo script, buyer cheat card. | "one-pager for YMCA directors" | v1.7.29 | Live in claude.ai |
| 17 | 15 | 2 | Agent 10 — Content Strategy | `daxko-content-planner` | Plans what content to make: content calendar, topic ideas, what is missing. | "content plan for Q1 for BGCs" | v1.7.30 | Live in claude.ai |
| 18 | 16 | 2 | Agent 15 — Email & Nurture | `daxko-email-nurture` | Writes or fixes an email-only series: nurture, welcome, re-engagement, win-back. | "nurture sequence for JCC leads" | v1.7.31 | Live in claude.ai |
| 19 | 17 | 2 | Agent 49 — Renewal & Expansion | `daxko-renewal-expansion` | For one existing customer: which Daxko add-on fits next and why, and how to prepare the renewal talk. | "expansion plan for this YMCA" | v1.7.32 | Live in claude.ai |
| 20 | 18 | 2 | Agent 57 — Sales Coaching | `daxko-sales-coaching` | Coaches a sales rep on one new-business call: plays a practice buyer, preps a call, or reviews a call you paste — what worked, what missed, what to say instead. | "practise a discovery call with me as a YMCA CFO" | v1.7.33 | Live in claude.ai |
| 21 | 19 | 2 (added) | Agent 12 — Blog & Article | `daxko-blog-writer` | Writes one search-optimized blog post for one market and segment from Daxko's files and blog guidelines — titles, meta description, the post with FAQs and a demo call to action — or an outline first, or a corrected version of an old post you paste. | "write a blog post for mid-size YMCAs about keeping members after January" | v1.7.35 | Live in claude.ai |

19 skills, 21 agents.

More agents are added over time, one tested agent at a time. This table is updated with every release.

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
