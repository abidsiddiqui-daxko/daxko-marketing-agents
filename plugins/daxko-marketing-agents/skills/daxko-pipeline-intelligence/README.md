# Daxko Pipeline Intelligence — Agent 22 — Pipeline Intelligence

**Version:** 1.10.1 · **Skill:** `daxko-pipeline-intelligence` · **Owner:** Abid Siddiqui · **Type:** read-only data analyst

## What it does, in plain words
Paste a pipeline export from Salesforce and ask how healthy it is. It works out 90-day coverage, deal speed, overdue and long-sitting deals and forecast vs actual — by market, segment and stage — and shows every sum.

## What to give it
One row per deal (account, market, new logo or expansion, stage, amount, created date, close date) with no contact details; the bookings target for the next 90 days; the period.

You can paste the numbers, or let it pull them through a connector you already have — it always asks first
("May I pull … read-only, for this task only?") and only goes ahead after you say yes.

## What it will never do
- Change anything in a live system (no deal, stage, amount, close date, forecast category, owner or note in Salesforce or any CRM).
- Invent a number, target or "industry benchmark".
- Repeat personal details (names, emails, phone numbers) — it leaves them out.
- Say a roadmap AI feature is live.
- Watch numbers over time or send alerts — it only runs when you ask.

## Example asks
- "Do we have 3x coverage for nonprofit new logo?"
- "Which deals are past their close date?"
- "Is deal velocity better than last quarter?"

## Who handles what instead
Marketing numbers vs a Key Result → Agent 18 — Marketing Performance · stage and scoring design → `daxko-revops` · one renewal → Agent 49 — Renewal & Expansion · one call → Agent 57 — Sales Coaching.

Corrections: send them to Abid Siddiqui, who adds a dated line to `learnings/agent-22-pipeline-intelligence.md`.
