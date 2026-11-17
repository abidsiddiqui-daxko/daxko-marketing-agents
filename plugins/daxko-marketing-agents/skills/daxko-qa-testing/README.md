# Agent 32 — QA & Testing — teammate guide

**Skill:** `daxko-qa-testing` · **Owner:** Abid Siddiqui · **Version:** 1.10.0

## What it does
Does-it-work checking (QA) for a website build — a Digital Services client's site or a Daxko web page. It writes test plans and test cases, turns a tester's notes into clear bug reports, and sums up a test round with a go / no-go recommendation for the project lead. It first asks up to 3 short questions: what is being tested, on which devices and browsers, and your team's bug format.

## Requests to try
- "Write test cases for the new YMCA site's join form"
- "Turn these tester notes into bug reports" (paste the notes)
- "Sum up this QA round — are we ready to launch?" (paste the results)

## Good to know
- It does not test the site itself and never opens, closes or changes a ticket. It reads tickets from a connector only if you say yes.
- It never marks a test passed that nobody reported, and never hides open bugs to make a date.
- Passwords or card numbers in your notes are left out, and it tells you to change a shared password.
- Its severity scale is a suggestion — use your team's if you have one.

## What it will NOT do — and who does
| Ask | Owner |
|---|---|
| Brand compliance | `daxko-brand-qa` |
| Accessibility (WCAG) review | Agent 43 — Accessibility |
| Ad campaign pre-launch checklist | Agent 73 — Pre-Launch QA |
| Daxko product bug trends | Agent 52 — Defect & Quality Intelligence |
| Page speed | `daxko-seo-audit` |
| Filing or closing tickets, launching | a human on the Digital Services team |
