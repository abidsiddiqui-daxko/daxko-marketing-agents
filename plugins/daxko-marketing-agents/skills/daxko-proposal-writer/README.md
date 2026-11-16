# Agent 58 — Proposal Generator — teammate guide

**Skill:** `daxko-proposal-writer` · **Owner:** Abid Siddiqui · **Version:** 1.8.0

## What it does
Drafts one sales proposal or one statement of work (SOW) for one deal. It first asks you up to 3 short questions — your deal notes, the approved prices from sales, and your template — then writes the draft from what you paste plus Daxko's files: what the buyer needs, which Daxko products fit, approved proof, how implementation works, next steps and a price section that only repeats the approved figures you pasted.

## Requests to try
- "Write a proposal for a mid-size YMCA" (then paste the deal notes)
- "Draft an SOW for this Club Automation deal" (paste your template)
- "Answer this RFP for a martial arts school group" (paste the questions)

## What you get
The draft under **DRAFT PROPOSAL — needs your sales sign-off and Agent 9 — Brand Guardian**, internal notes kept apart, what it declined and who owns it, a NOT ON FILE list and sources with dates.

## Good to know
- No price from Daxko's files. Prices appear only when you paste the approved figure — repeated exactly, never discounted or rounded.
- It can pull one opportunity from your CRM connector, but only after asking you and only read-only. Otherwise paste the notes.
- Leave out names, emails and phone numbers; it never repeats personal or sensitive details.
- No legal terms, go-live dates or roadmap AI. It sends, signs and updates nothing.

## What it will NOT do — and who does
| Ask | Owner |
|---|---|
| One-pager, deck outline, discovery guide | Agent 21 — Sales Enablement |
| ROI calculator | `daxko-sales-enablement` |
| What to charge, discounts | `daxko-pricing-strategy` · sales |
| Renewal or upsell plan | Agent 49 — Renewal & Expansion |
| Objection answers | Agent 20 — Battlecard & Objection Handling |
| New customer proof | Agent 67 — Customer Proof & Advocacy |
| Legal terms · go-live dates | Daxko's legal team · Daxko's implementation team |
| Word or PDF file | `docx` · `pdf` |
| Follow-up sequence | `gong-sequence-builder` (your own skill) |
| Send it, e-sign, update the CRM | a human |
