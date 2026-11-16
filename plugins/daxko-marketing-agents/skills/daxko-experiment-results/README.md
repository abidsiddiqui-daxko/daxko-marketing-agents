# Daxko Experiment Results — Agent 53 — Experiment & Feature Flag

**Version:** 1.8.0 · **Skill:** `daxko-experiment-results` · **Owner:** Abid Siddiqui · **Type:** read-only data analyst

## What it does, in plain words
Paste the results of an A/B test or a feature-flag rollout. It checks whether the difference is real — enough people, a significance test worked out step by step, side effects — and says ship, stop or keep running, for a person to decide. It can also spot old flags to clean up.

## What to give it
Users and conversions per variant with dates (or averages with spread and counts); the main metric chosen before the test; any planned sample size; for flags, a list with state, dates and owning team.

You can paste the numbers, or let it pull them through a connector you already have — it always asks first
("May I pull … read-only, for this task only?") and only goes ahead after you say yes.

## What it will never do
- Change anything in a live system (no feature flag turned on or off, no rollout percentage changed, no test started, stopped or re-targeted).
- Invent a number, target or "industry benchmark".
- Repeat personal details (names, emails, phone numbers) — it leaves them out.
- Say a roadmap AI feature is live.
- Watch numbers over time or send alerts — it only runs when you ask.

## Example asks
- "Did variant B win?"
- "Is this email subject-line result significant?"
- "Which feature flags can we clean up?"

## Who handles what instead
Designing a test → `daxko-ab-test-setup` · tracking → `daxko-analytics-tracking` · page advice → `daxko-page-cro` · Key Result roll-up → Agent 18 — Marketing Performance.

Corrections: send them to Abid Siddiqui, who adds a dated line to `learnings/agent-53-experiment-results.md`.
