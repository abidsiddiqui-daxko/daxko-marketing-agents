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
skill #12, which is why there are 58 rows but only 56 skills. *Ask it like this* is copied from the
skill's own description. *First published* is checked against the plugin repo's git history.
*Batch 1* skills are out with stakeholders for testing and are not changed; *Batch 2* and *Batch 6* skills are live.

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
| 22 | 20 | 6 | Agent 45 — CX Email & Response | `daxko-support-reply` | Drafts one reply to one customer support email or case you paste (or one reusable response template, or fixes your draft reply), for you to check and send. | "draft a reply to this upset YMCA director about a double charge" | v1.7.36 | Live in claude.ai |
| 23 | 21 | 6 | Agent 46 — Knowledge Base & Article | `daxko-help-article` | Writes one help-center article, FAQ or how-to from the steps or answer you paste — screen and button names exactly as given; never invents a menu or button. | "help article on setting up family billing in Daxko Operations from these steps" | v1.7.36 | Live in claude.ai |
| 24 | 22 | 6 | Agent 48 — Success Playbook & QBR | `daxko-success-qbr` | Builds a quarterly business review (QBR) outline or a success plan for one existing customer account from facts you paste, or a success playbook for one segment. | "QBR outline for the Testville YMCA" | v1.7.36 | Live in claude.ai |
| 25 | 23 | 6 | Agent 58 — Proposal Generator | `daxko-proposal-writer` | Drafts one sales proposal, SOW or RFP response for one deal from your pasted deal notes; prices only as sales gave them. | "write a proposal for this mid-size YMCA" | v1.7.36 | Live in claude.ai |
| 26 | 24 | 6 | Agent 1 — AI Strategy & Governance | `daxko-ai-governance` | Answers "can I use this AI tool or paste this data?" from Daxko's AI rules and the Safe Harbor draft — fits, breaks, or ask Information Security; never says "approved". | "can I paste our member export into Claude?" | v1.7.36 | Live in claude.ai |
| 27 | 25 | 6 | Agent 43 — Accessibility | `daxko-accessibility` | Checks one pasted web page, form or email for things that block disabled people, says how to fix each, writes alt text and works out colour contrast. | "is this form screen-reader friendly?" | v1.7.36 | Live in claude.ai |
| 28 | 26 | 6 | Agent 26 — Client Communication | `daxko-client-updates` | Drafts one message to a Digital Services client — status update, meeting recap, reply or request — from pasted notes; never sends. | "write this week's status update for our YMCA website client" | v1.7.36 | Live in claude.ai |
| 29 | 27 | 6 | Agent 25 — Onboarding & Requirements | `daxko-client-requirements` | Writes kickoff questions for a new web client, or turns their answers into a project brief with scope, owners and open questions. | "turn these intake answers into a project brief" | v1.7.36 | Live in claude.ai |
| 30 | 28 | 6 | Agent 73 — Pre-Launch QA | `daxko-ad-prelaunch-check` | Checks one ad campaign's settings against its brief before it goes live and says GO or NO-GO; changes nothing. | "is this Meta campaign ready to launch?" | v1.7.36 | Live in claude.ai |
| 31 | 29 | 6 | Agent 27 — Strategy & Discovery | `daxko-client-discovery` | Discovery questions, a review of a client's local competitors from pasted pages, and a short digital strategy for one Digital Services client. | "compare our client's site with these two local clubs" | v1.7.36 | Live in claude.ai |
| 32 | 30 | 6 | Agent 35 — Web Content | `daxko-web-content` | Writes website copy for a Digital Services client's own site — up to 3 pages, a client blog post, a rewrite, or page titles and metas — from the client facts you paste. | "write the homepage for the Riverbend YMCA's new site" | v1.7.36 | Live in claude.ai |
| 33 | 31 | 6 | Agent 71 — Budget Reallocation | `daxko-budget-reallocation` | Recommends where a Digital Services client's ad money should move between campaigns, from numbers you paste (or reads with your OK) — never moves money itself. | "should we shift budget from Meta to Google for this YMCA client" | v1.7.36 | Live in claude.ai |
| 34 | 32 | 6 | Agent 28 — Information Architecture | `daxko-information-architecture` | Plans a website's page tree, menus and web addresses — for a client's site or a Daxko site — plus an old-to-new address map when a site is rebuilt. | "plan the sitemap for a JCC's new website" | v1.7.36 | Live in claude.ai |
| 35 | 33 | 6 | Agent 32 — QA & Testing | `daxko-qa-testing` | Does-it-work checking for a website: test plans and cases, bug reports from a tester's notes, and a go / no-go summary — tests nothing live itself. | "turn these tester notes into bug reports" | v1.7.36 | Live in claude.ai |
| 36 | 34 | 6 | Agent 6 — Pendo Engagement Intelligence | `daxko-usage-insights` | Reads a product-usage export (Pendo or similar) and says which features customers use or ignore, what changed, and which accounts look busy or quiet. | "which Club Automation features are customers not using?" | v1.7.36 | Live in claude.ai |
| 37 | 35 | 6 | Agent 22 — Pipeline Intelligence | `daxko-pipeline-intelligence` | Reads a Salesforce pipeline export and works out 90-day coverage, deal speed, overdue deals and forecast vs actual, by market, segment and stage. | "do we have 3x coverage for nonprofit new logo?" | v1.7.36 | Live in claude.ai |
| 38 | 36 | 6 | Agent 17 — Paid Media | `daxko-paid-media` | Reads results of Daxko's own Google, LinkedIn and Meta ads and says what worked, what didn't, and what a person could pause, scale or test. | "how did our LinkedIn ads do last month?" | v1.7.36 | Live in claude.ai |
| 39 | 37 | 6 | Agent 52 — Defect & Quality Intelligence | `daxko-defect-quality` | Reads a bug export (Jira or similar), release dates and support numbers and shows where bugs cluster, how fast critical bugs get fixed and how stable releases were. | "are we fixing S1 and S2 bugs within 30 days?" | v1.7.36 | Live in claude.ai |
| 40 | 38 | 6 | Agent 53 — Experiment & Feature Flag | `daxko-experiment-results` | Reads A/B test or feature-flag results and says whether the difference is real (worked out step by step) — ship, stop or keep running, for a person to decide; spots stale flags. | "did variant B win?" | v1.7.36 | Live in claude.ai |
| 41 | 39 | 6 | Agent 16 — AI Lifecycle Orchestration | `daxko-lifecycle-journeys` | Plans one customer journey — onboarding, adoption, retention or expansion — for Daxko's own customers from usage you paste: what starts each step, what it's for, when, which channel, who owns it. Writes no emails and sends nothing. | "onboarding journey for new Club Automation customers" | v1.7.37 | Live in claude.ai |
| 42 | 40 | 6 | Agent 29 — UX/UI Design | `daxko-ux-design` | Lays out a website's pages in words — wireframes, the parts the site needs and a simple style guide — for a Digital Services client (or a Daxko page if asked), from the brand you paste. No pictures or code. | "wireframe the homepage for our YMCA client's new site" | v1.7.37 | Live in claude.ai |
| 43 | 41 | 6 | Agent 34 — SEO & AEO | `daxko-site-seo` | Gives one website — a Digital Services client's, or Daxko's own if asked — an ordered list of fixes so it shows up better on Google and in AI answers like ChatGPT, from the Search Console or Analytics numbers you paste. Changes nothing on the site. | "SEO fixes for this YMCA client's site from this Search Console export" | v1.7.37 | Live in claude.ai |
| 44 | 42 | 6 | Agent 39 — CRO | `daxko-site-conversion` | Reads one website's visitor numbers (Google Analytics, Clarity), finds where people drop out before becoming leads, and recommends changes in order — never edits the site or starts a test. | "our YMCA client gets 9,000 visits but only 40 tour bookings - why" | v1.7.37 | Live in claude.ai |
| 45 | 43 | 6 | Agent 40 — Client Success | `daxko-client-health` | Health check for one Digital Services client — rates each warning sign green, amber or red with the evidence, says what's at risk and who acts; can rank a list of clients. | "health check for our YMCA website client" | v1.7.37 | Live in claude.ai |
| 46 | 44 | 6 | Agent 41 — Retention & Upsell | `daxko-client-retention-upsell` | For one Digital Services client: the next service that fits, or a save plan if they may cancel — no prices or discounts unless sales pastes them. | "this club client wants to cancel their SEO - save plan" | v1.7.37 | Live in claude.ai |
| 47 | 45 | 6 | Agent 42 — Speed & Performance | `daxko-site-speed` | Reads a pasted PageSpeed or Lighthouse report for one website and lists the speed fixes in order, each tied to a line in the report — tests and changes nothing itself. | "what should we fix first from this PageSpeed report" | v1.7.37 | Live in claude.ai |
| 48 | 46 | 6 | Agent 8 — CMO Orchestrator | `daxko-cmo-orchestrator` | For one goal or campaign, says which of our agents to use and in what order, what each needs and hands on, where the brand check sits, and which Key Result it serves. Does no agent's work; after your yes it can add the steps as tasks in your Asana project. | "which agents should we use for the Giving Tuesday push" | v1.8.0 | Live in claude.ai |
| 49 | 47 | 6 | Agent 24 — Agency Orchestrator | `daxko-project-delivery` | Runs one Digital Services client project — plan by stage, what's late or blocked, next week's actions, internal status; can create Asana tasks after your yes. | "plan the Asana tasks for this YMCA website build" | v1.8.0 | Live in claude.ai |
| 50 | 48 | 6 | Agent 30 — Frontend Development | `daxko-frontend-spec` | Turns one web page or template into a build spec in plain words for the web publishing team — sections, what goes in each slot, how it behaves, phone / tablet / desktop rules, accessibility needs and "done when" checks. Writes no code; after your yes it can put the spec in one Asana task or doc. | "build spec for our YMCA client's new homepage" | v1.8.0 | Live in claude.ai |
| 51 | 49 | 6 | Agent 31 — Backend/CMS | `daxko-cms-setup` | Plans one client site's CMS setup — content types, fields, roles, forms, links, plugins, checklist; can create draft items after your yes. | "CMS setup plan for our YMCA client's new WordPress site" | v1.8.0 | Live in claude.ai |
| 52 | 50 | 6 | Agent 33 — Content Migration | `daxko-content-migration` | Moves one client site's old pages to the new site — inventory, move map, cleaned text, redirect list, checks; can create draft pages after your yes. | "move the old site's pages into the new site" | v1.8.0 | Live in claude.ai |
| 53 | 51 | 6 | Agent 36 — Paid Digital | `daxko-client-ads` | Builds one new ad campaign for a Digital Services client — structure, targeting, budget and dates as given, keywords as pasted, ad text, names and tracking tags — and, after your yes, can create it paused in their ad account. Never turns ads on or spends money. | "build the Google Ads campaign for our YMCA client's spring drive" | v1.8.0 | Live in claude.ai |
| 54 | 52 | 6 | Agent 37 — Social Media | `daxko-client-social` | Plans and writes one client's social calendar — dates, platforms, post text, image notes, approval list — and, after your yes, can load the posts as unscheduled drafts. Never schedules or posts. | "social calendar for our YMCA client for March" | v1.8.0 | Live in claude.ai |
| 55 | 53 | 6 | Agent 56 — Campaign Workflows | `daxko-campaign-golive` | Makes every channel of one Daxko campaign go live together — run-sheet, owners, a ready check per channel, go / no-go, slip plan — and, after your yes, can create internal Asana tasks and post one internal Slack message. Never sends, launches or publishes. | "launch checklist for our Q1 campaign across email, ads and social" | v1.8.0 | Live in claude.ai |
| 56 | 54 | 6 | Agent 23 — Event & Webinar (event messaging) | `daxko-event-promotion` | Writes the promotion for one Daxko event or webinar — emails, sales sequence, social, landing page, Pendo, blogs, sponsor and booth copy, webinar invites and follow-up — and, after your yes, can save unsent drafts in HubSpot or Salesloft. Never sends or publishes. | "event assets for NAYDO — emails, sales sequence and social" | v1.9.0 | Live in claude.ai |
| 57 | 55 | 6 | Agent 23 — Event & Webinar (event planning) | `daxko-event-planning` | Plans one Daxko event or webinar from contract to recap — brief, Slack setup, team selection, travel emails, workback, kickoff deck, canvases, week-of messages, organizer deliverables, field guide, webinar run of show and the Event ROI score — and, after your yes, can create internal Asana tasks, post one internal Slack message or save an internal document. Never books, buys, emails or submits. | "we just signed for IHRSA, set it up" | v1.9.0 | Live in claude.ai |
| 58 | 56 | 7 | Agent 19 — BDR/AM Sequence Builder | `daxko-outbound-sequences` | Writes outreach that Daxko reps send themselves — one cold email, or a prospecting or customer sequence in only the channels asked for (email only, calls only, LinkedIn only, or a mix) — after asking short rounds of questions. Approved proof only; never invents stats, customers, quotes, prices or roadmap AI; never sends or enrolls. | "BDR sequence for JCCs" | v1.10.0 | Live in claude.ai |

56 skills, 57 agents (Agent 23 — Event & Webinar has two skills).

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
