# Agent 73 — Pre-Launch QA — teammate guide

**Skill:** `daxko-ad-prelaunch-check` · **Owner:** Abid Siddiqui · **Version:** 1.8.0

## What it does
Checks one paid ad campaign before it goes live — for a Digital Services client or for Daxko itself, on Google, Meta, LinkedIn or another platform. You paste the campaign settings and the approved brief (or, if you say yes, it reads the settings from a connector you already have). It compares them line by line and gives a go / no-go checklist: naming, UTM tags, conversion tracking, landing page link, targeting, budget and dates, and red flags in the ad text. Each line is Pass, Fix or Not given, with the evidence, plus a plain fix list.

## Requests to try
- "Pre-launch QA on this Google Ads campaign" (paste settings and brief)
- "Check these UTMs and the budget before we go live"
- "Is this Meta campaign for our YMCA client ready to launch?"
- "Go / no-go on our LinkedIn campaign, it starts Monday"

## What you get
A verdict (GO, NO-GO or CAN'T TELL YET), the checklist table and a fix list under **DRAFT — needs the campaign owner before anything goes live**, then internal notes, what it declined and who owns it, a NOT ON FILE list and sources with dates.

## Good to know
- If you haven't pasted the settings, the brief or whose campaign it is, it asks you up to 3 short questions first.
- No naming convention is on file — paste yours, or it only checks the names are consistent with each other.
- It shows the budget math (daily × days vs approved total). It cannot open the landing page — it checks the link only.
- For Daxko's own ads it flags prices, roadmap AI (such as Smart Sending Engine) written as live, "#1" claims and banned words.
- It never launches, pauses, edits or re-budgets anything — the campaign owner does that. Audience lists: counts only.

## What it will NOT do — and who does
| Ask | Owner |
|---|---|
| Set up tracking or a UTM plan | `daxko-analytics-tracking` |
| Campaign strategy or targeting advice | `daxko-paid-ads` |
| New ad copy | `daxko-ad-creative` |
| Brand verdict on Daxko's ad text | Agent 9 — Brand Guardian |
| Daxko's own live ad results | Agent 17 — Paid Media |
| Moving a client's live budget | Agent 71 — Budget Reallocation |
| Test whether the landing page works | Agent 32 — QA & Testing |
| Tell the client about the launch | Agent 26 — Client Communication |
| Gong or multi-touch sequence | `gong-sequence-builder` (your own skill) |
| Launch, pause or change the campaign | a human — the campaign owner |
