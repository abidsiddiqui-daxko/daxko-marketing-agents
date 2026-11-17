# Agent 16 — AI Lifecycle Orchestration — teammate guide

**Skill:** `daxko-lifecycle-journeys` · **Owner:** Abid Siddiqui · **Version:** 1.10.0

## What it does
Plans one customer journey for Daxko's own customers — onboarding, adoption, retention or expansion — for one product, segment or group of accounts. You paste account-level usage (for example a Pendo export), or, if you say yes, it reads it from a connector you already have. It lays out each step: what starts it, the message's purpose, when, on which of your channels, who owns it, when to stop — and what to measure against the GRR Key Result.

## Requests to try
- "Onboarding journey for new Club Automation customers"
- "Adoption journey for YMCAs not using online registration" (paste the usage)
- "Retention journey for accounts whose logins dropped"

## Good to know
- It plans only. It writes no emails (Agent 15 — Email & Nurture does) and builds, schedules or sends nothing.
- It uses only the channels you say you have, and only account-level numbers — never one person's activity.
- Thresholds and timings you didn't give are labelled "general practice, not a Daxko rule".
- It never says roadmap AI (like Smart Sending Engine) is available, and never promises a GRR lift.

## What it will NOT do — and who does
| Ask | Owner |
|---|---|
| Write the emails | Agent 15 — Email & Nurture |
| Explain a usage export | Agent 6 — Pendo Engagement Intelligence |
| One account's renewal | Agent 49 — Renewal & Expansion |
| In-app onboarding screens | `daxko-onboarding-cro` |
| Cancel flows, save offers | `daxko-churn-prevention` |
| Building or sending it | a human on the customer success or lifecycle marketing team |
