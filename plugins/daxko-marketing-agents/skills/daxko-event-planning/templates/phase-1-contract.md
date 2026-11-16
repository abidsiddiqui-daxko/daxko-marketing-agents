# Phase 1 templates — at contract signing

> SKILL VERSION: 1.9.0 · Used by `daxko-event-planning` (Agent 23 — Event & Webinar, event planning). Fill only with facts the person gave; every unknown is **TBD**. Contact details (email, phone) are never filled in — leave the placeholder. Shipping addresses and accounts are never filled from memory.

---

## 1. EVENT BRIEF

Same standard for every event, whatever its size. Offer it as a .docx when a Word-document tool is available in the chat (`[EventName]-EventBrief-[Year]`), otherwise markdown. Label: **DRAFT — event plan for internal use; needs the event manager's OK before anyone acts on it**

```
EVENT BRIEF · DAXKO FIELD MARKETING · [YEAR]
[Event Name]
[Date range, weekdays checked] · [Venue], [City, State]

[Quick stats: sponsorship tier · budget · booth size · brands represented · Tier 1 / Tier 2 (provisional if unconfirmed)]

WHY WE'RE HERE
[2–3 paragraphs of strategic rationale: why this event matters for the market, who the audience is, why Daxko's presence matters, what unique opportunity exists. Confident, strategic, specific — but every fact as pasted or from Daxko's files with its file named; no invented audience numbers. Competitive context only if competitors are confirmed attending.]

[Up to 4 reason cards, only those that apply: High-intent audience · Competitive battleground · Market opportunity · Multi-brand opportunity]

COMPETITIVE LANDSCAPE   ← only if competitors are confirmed attending
[Per competitor: 2–3 factual sentences from competitive-intel.md (its section named, compare on merits) and their likely floor presence as pasted, or TBD]

EVENT OVERVIEW
[1–2 sentences: what the event is and who attends — from what the person pasted or the event website text they pasted]

BRANDS REPRESENTED
[Daxko / Club Automation / Daxko Operations / Zen Planner / Exercise.com / SugarWOD — only those that apply]

BOOTH DETAILS
Size: [size] | Booth #: [# or TBD] | Setup: [date + time or TBD] | Teardown: [date + time or TBD]
[Floorplan note if available]

SPONSORSHIP INCLUSIONS
[Bullets, per contract as pasted]

SCHEDULE
| Date | Time | Activity |   ← from the agenda; TBD where unknown

TEAM ATTENDING
[Names and roles as given, or: "No teammates confirmed yet — add names before sharing with Creative"]

EVENT ORGANIZER CONTACT
[Name, title, company as given] · [organizer email / phone — add from your records]

LINKS & RESOURCES
Asana board | OneDrive folder | Salesforce campaign | HubSpot emails | Attendee list | Event website — each [link or TBD]

KEY RESULT
[Quoted word for word from okrs-and-priorities.md, or [needs: which Key Result — event manager]]
```

---

## 2. SLACK CHANNEL SETUP

The person creates the channel and canvases (this skill never creates a channel or canvas). After a yes and with a connector, it may post the pinned message in a channel the person confirms is internal (SKILL.md, CHANGE LIST).

```
SLACK CHANNEL SETUP — [Event Name] [Year]

Channel name: event-[event-name-abbreviated]-[year]
Examples: event-naydo-2026, event-hfa-2026, event-community-rec-summit-2026

CANVASES TO CREATE (create these yourself inside the channel — templates in Phase 3):
□ Event Brief — paste the completed event brief
□ Shipping / Venue Info + Tracking Numbers — update as info comes in
□ Popl Instructions — standard lead-capture instructions
□ Planning Sync Agenda — running doc for the recurring planning meeting, if there is one

FIRST MESSAGE IN THE CHANNEL (pin it — update it as info comes in):
---
📌 [Event Name] — Key Info

Dates: [event dates]
Location: [state + venue]
Team Attending: [names or TBD]
Prep Meeting: [date + time or TBD]
Sponsorship: [one-line summary, e.g. "5 min speaking slot + exhibitor table"]

Links:
• Event Brief: [link or TBD]
• Event Site: [link or TBD]
• Salesforce Campaign: [link or TBD]
• Asana Board: [link or TBD]
---

After setup: add all relevant stakeholders to the channel.
```

---

## 3. TEAM SELECTION

**Format by tier and market:** Tier 2 → Slack message · Tier 1 → formal email · single market → only that market's sales leader(s) · multi-market → one message to all relevant leaders, saying which reps are needed from each org. Sales-org mapping: Club → Club Automation sales leaders · Nonprofit → Daxko Operations sales leaders · Boutique → Boutique sales leaders (by segment if relevant). Nomination deadline: **~6–8 weeks before the event** (Field Marketing standard timing) — counted from the pasted start date, weekday checked. A draft only — the event manager sends it.

**Tier 2 — Slack message**
```
Hey [@ sales leader(s)]! We're contracted for [Event Name] — [dates], [city, state].

[If multi-market: This event draws attendees across [markets]. We need reps from each team — [orgs].]

We can send up to [#] people. Could you let me know by **[deadline]** who you'd like to attend? Hotel booking deadline is **[date or TBD]**.

Participation includes:
• [inclusions as pasted]

[If an attendee list is available: Here's the current / prior-year attendee list to help you pick who should attend by territory: [link]]
[If not: We don't have the attendee list yet — I'll share it once available.]
```

**Tier 1 — formal email**
```
Subject: [Action Required] Team Nominations for [Event Name] — [Dates]

Hi [sales leader name(s) or role(s)],

We're confirmed for [Event Name] ([dates]) in [city]. [If multi-market: This event serves [markets], and we need representation from each sales org.]

Sponsorship includes:
• [inclusions as pasted]

[If multi-market: Here's what we need from each team:
• Club Automation: [# reps or TBD]
• Daxko Operations: [# reps or TBD]
• Boutique: [# reps or TBD]]
[If single market: We have [#] spots available for the [market] team.]

Please nominate your reps by **[deadline]**. Travel booking opens right after confirmation, so early nominations help lock in better flights.

[If an attendee list is available: Prior attendee list attached for territory reference.]

Let me know if you have questions.

[Sender name]
Event Manager, Daxko
```

---

## 4. TRAVEL EMAILS

Three versions — **chosen by role, not event size**. Voice: the event manager's — direct, warm, action-oriented, **deadlines in bold**. Booking deadline: **~6–8 weeks before the event** (Field Marketing standard timing), counted and weekday-checked. Drafts only — the event manager sends them; nobody's flight or room is booked by this skill. Write "a block is secured" only if the person said it is secured; if they asked you to book it, write `[room block — confirm it is secured]`. Figures (goals, budgets) are copied exactly as typed — no added currency sign or unit. No traveller's personal details (passport, home address, loyalty or confirmation numbers) ever go in an email.

**Executive travel (VPs, C-suite — they have EAs)**
```
Subject: [Action] Book Travel to [Event Name]

Hey team,

It's time to book your flight to [Event Name]! This year's [short event name] will be [dates] in [city].
[Link to the conference schedule, if available]

Rooms are currently held for each of you from [date range]. Please book your flights and let me know if you'd like to shorten your stay so I can adjust your hotel.

EA action needed: please book flights by **[deadline]**. Once booked, please fill out this sheet with the team's travel details: [link or TBD]

Recommended arrival timing, based on [speaking / meeting] schedules:

| Name | Recommended arrival | [Session / meeting] |
|------|---------------------|---------------------|
| [Name as given] | [Date — anytime] | [Date + time or TBD] |

The first agenda item for the full team is [first team activity, e.g. booth rehearsal] at [time] on [date].
[The event / booth closes at [time] on [date].]

You do not need to book a hotel. A room block is secured at [hotel name], and I'll share confirmation numbers with your EAs once received.

Let me know if you have questions!
```

**Tier 1 staff travel (booth team, larger events — hotel already blocked)**
```
Subject: [Action] Book Your [Event Name] Flight

Hey team,

It's time to book your flight to [Event Name]!
This year's event will be [dates] in [city].
[Link to the conference schedule]

Action needed: please book your flight by **[deadline]**. Once booked, fill out this sheet with your travel details: [link or TBD]

Flight requirements (book using Egencia):
Location: [city] | [venue name + address as pasted, or TBD]
• Arrive **[date] by [time]** ([reason — e.g. first agenda item is booth rehearsal at X; allow time to settle in])
• Depart **[date] after [time]** ([reason — e.g. the booth closes at X; make sure your flight doesn't conflict])
• Expense report: please expense your travel to your own team

Hotel requirements:
You do not need to book your hotel. A block is secured at [hotel name], and I'll share confirmation numbers in our #[slack-channel-name] Slack channel once received.

Upcoming team trainings:
[List any scheduled — booth meetings training, run-of-show walkthrough, Popl training — or remove this section if none yet]
Stay tuned for dates and details. Drop questions in #[slack-channel-name] or Slack me directly.
```

**Tier 2 staff travel (smaller events — hotel self-book)**
```
Subject: [Action] Book travel for [Event Name]

Team —

It's time to book travel for [Event Name]! This year's event will be [dates] in [city, state].

Action needed: please book your flight and hotel by **[deadline]**.

Flight requirements (book using Egencia):
Location: [city] | [hotel name + address as pasted, or TBD]
• Arrive **[date] [anytime / by time]** ([setup note — e.g. setup is the morning of X; the conference begins at noon])
• Depart **[date] after [time]** ([breakdown note — e.g. booth breakdown begins at noon])
• Expense report: please expense your travel to your own team

Hotel requirements (book using the link below):
You'll be staying at: [hotel name + address as pasted, or TBD]
[Hotel booking link or TBD]
Please use the link to book your hotel. You'll pay on your personal card and expense it to your team.

Let me know if you have any questions,
```
