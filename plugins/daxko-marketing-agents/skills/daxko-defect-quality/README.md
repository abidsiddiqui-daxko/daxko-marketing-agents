# Daxko Defect & Quality — Agent 52 — Defect & Quality Intelligence

**Version:** 1.9.0 · **Skill:** `daxko-defect-quality` · **Owner:** Abid Siddiqui · **Type:** read-only data analyst

## What it does, in plain words
Paste a bug export from Jira (plus release dates or support-case counts) and ask where the problems are. It shows where bugs cluster, how fast critical bugs get fixed, how stable releases were and how support numbers move — every sum shown.

## What to give it
One row per bug (ID, product, component, severity, created date, production-fix date, release, status) without customer details; release dates; the period.

You can paste the numbers, or let it pull them through a connector you already have — it always asks first
("May I pull … read-only, for this task only?") and only goes ahead after you say yes.

## What it will never do
- Change anything in a live system (no ticket created, edited, commented on, assigned, re-prioritised, re-labelled or closed in Jira or any tracker).
- Invent a number, target or "industry benchmark".
- Repeat personal details (names, emails, phone numbers) — it leaves them out.
- Say a roadmap AI feature is live.
- Watch numbers over time or send alerts — it only runs when you ask.

## Example asks
- "Are we fixing S1 and S2 bugs within 30 days?"
- "How stable was the October release?"
- "Which product has the most open defects?"

## Who handles what instead
Ticket text themes → Agent 50 — Product Insights & Feedback · client website QA → Agent 32 — QA & Testing · release briefings → Agent 51 — Roadmap & Release Briefing · a customer reply → Agent 45 — CX Email & Response.

Corrections: send them to Abid Siddiqui, who adds a dated line to `learnings/agent-52-defect-quality.md`.
