# Daxko Usage Insights — Agent 6 — Pendo Engagement Intelligence

**Version:** 1.9.0 · **Skill:** `daxko-usage-insights` · **Owner:** Abid Siddiqui · **Type:** read-only data analyst

## What it does, in plain words
Paste a Pendo (or similar) usage export and ask what it means. It tells you which features customers use or ignore, what changed and when, which accounts look busy or quiet, and what marketing, sales and customer success could check next.

## What to give it
Account-level usage counts by feature or page, with dates; the product, market and period; what you most want to know.

You can paste the numbers, or let it pull them through a connector you already have — it always asks first
("May I pull … read-only, for this task only?") and only goes ahead after you say yes.

## What it will never do
- Change anything in a live system (no Pendo guide, segment, tag, poll or account record; no message to any customer).
- Invent a number, target or "industry benchmark".
- Repeat personal details (names, emails, phone numbers) — it leaves them out.
- Say a roadmap AI feature is live.
- Watch numbers over time or send alerts — it only runs when you ask.

## Example asks
- "What does this Pendo export tell us about Club Automation V2?"
- "Which features are customers not using?"
- "Which accounts went quiet this quarter?"

## Who handles what instead
One account's renewal → Agent 49 — Renewal & Expansion · one account's QBR → Agent 48 — Success Playbook & QBR · customer comments → Agent 50 — Product Insights & Feedback · onboarding flows → `daxko-onboarding-cro`.

Corrections: send them to Abid Siddiqui, who adds a dated line to `learnings/agent-06-usage-insights.md`.
