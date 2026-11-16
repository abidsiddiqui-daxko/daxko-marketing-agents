> **SOURCE:** example file inside the Field Marketing skill `daxko-event-comms` (file in Abid Siddiqui's Downloads, July 2026) · **LAST UPDATED:** 2026-11-16 · **ORIGIN:** copied for Agent 23 — Event & Webinar (Batch 6 round 4); named speakers replaced with their roles · **Placed in Agent HQ:** 2026-11-16
> **Use:** format, structure and length examples only. Event names, dates, stats and offers in these examples are from past events — never reuse them as facts for a new event.

# Sales Sequence Examples

Load this file when generating 4B (Sales Outreach Sequence) assets. Mirror the format, structure, tone, send-type labeling, token format, and document organization shown below.

---

## Format Standards (apply to every sequence)

### Send Type Icons
Label every email and call step with its send type. Use these exact labels:

- **✋ MANUAL** — Rep sends personally. Rep must review and customize before sending.
- **⚡ AUTOMATED** — Triggered automatically by timing or enrollment logic. MOPs must send a test before deploying.

All emails default to **✋ MANUAL** unless the user explicitly requests automation. When a step is automated, always add the `🧪 MOPS TEST REQUIRED` flag and a test instruction.

### Token / Placeholder Format
All personalization fields use `{curly braces}`. No other bracket styles. Examples:
- `{First Name}`, `{Rep First Name}`, `{Rep Name}`, `{Rep Phone Number}`
- `{Gym Name}`, `{Company Name}`, `{Organization Name}`
- `{One specific thing from the conversation}` — free-text field the rep fills in personally
- `{Day}`, `{Time}` — booking confirmation fields
- `{rep@brand.com}` — rep's send-from address

Every sequence must end with a **Token Reference table** listing every token used, its meaning, and which steps it appears in.

### Sequence at a Glance Table
Open every sequence with a summary table:

```
| Step | Type | Timing | Goal |
|---|---|---|---|
| Email 1 | ✋ MANUAL | [when] | [one-line goal] |
| Call 1  | ✋ MANUAL | [when] | [one-line goal] |
| Email 2 | ⚡ AUTO  | [when] | [one-line goal] |
...
```

### Call Step Format
For every call step, include:
- **If They Answer** section with opening, branching script (IF/THEN), and book-on-the-call instruction
- **Objection Handling** section (2–4 common objections with responses)
- **Voicemail** script (leave if no answer; 30–45 seconds; ends with callback number)
- **Fallback** note: what to do if no answer (always: leave voicemail, move to next step)

Key rule on calls: **Book the time on the call. Do NOT send a scheduling link and wait.** If they agree to meet, get a specific day and time, confirm it out loud, and send the calendar invite immediately after hanging up.

### Automated Email Requirements
For every ⚡ AUTOMATED email, include:
- Trigger condition (e.g., "14 days before event AND no booking logged for contact")
- Send-from note (send-from maps to rep's address so replies land with them)
- `🧪 MOPS TEST REQUIRED` flag with specific test instructions

### MOPs Checklist
Every sequence ends with this block (required, never omit):

> **📋 MOPs Checklist — Before This Sequence Goes Live:**
> - [ ] Review send type on each step (all default to Manual — confirm any Automated sends are intentional)
> - [ ] Send a test of every email; confirm formatting, links, and all `{tokens}` render correctly
> - [ ] Confirm send-from address on automated emails maps to the correct rep
> - [ ] Review all copy one final time against the approved messaging framework or market voice
> - [ ] Confirm all `{tokens}` are either pre-populated by data or flagged for rep to fill before sending
> - [ ] QA automated trigger conditions (timing, enrollment criteria, exit/unenrollment logic)

---

## Tier 1 Events: Pre-Booked Meetings Process Document

When the event is Tier 1 (large budget, major pre-scheduled meeting push, multiple rep roles involved), generate a **Pre-Booked Meetings Process** document in addition to the sequence. This is a separate reference doc for the sales team — not part of the sequence itself.

**Ask the user:** "Is this a Tier 1 event with a structured pre-booked meeting push? If so, I'll generate a separate meetings process doc alongside the sequence."

### Meetings Process Document Format

The document covers:

**Meeting Types** — list each type with time block and rep expectations:
- Current Customer meetings (30–60 min): Rep comes prepared on account status; product team may join for roadmap discussion
- Strategic Prospect meetings (30–60 min): Rep has BANT established; demo of core product + suite; ELT or Product lead may be present
- Cold / New Prospect meetings (30–60 min): BDR sets the meeting; AE runs discovery in booth; establish pain points and next steps

**Talk Track reference:** Link to or embed the sales talk track (see Talk Track format below)

**When to use the outreach sequence:**
- Customers + Strategic Prospects → AEs use their respective scripts
- Cold / New Prospects → BDRs use BDR outreach scripts for landing page inbounds

**How to use it:**
1. Start with a live call when possible
2. Use email follow-ups only if: you miss them live / they request more info / they asked to follow up closer to event
3. Always frame meetings as: strategic conversations, focused on their priorities, not a generic demo

**How the Landing Page Works:**
- For Tier 1 events, the landing page uses a "Request a Meeting" form (not a direct calendar link) for 30–60 min strategic meetings
- After submission: request routes to Slack channel → BDRs review and route by meeting type → AE confirms availability → meeting officially booked
- Note the Slack channel name once confirmed

**Adding ELT/Product/Services to Meetings:**
- Process for requesting executive or product attendance
- Who approves, how to add to invite, any capacity limits

---

## Example A: CFG 2026 Pre-Event Sequence (Boutique / SugarWOD)

**Context:** Pre-event sequence for CrossFit Games Week. Goal: book owners and coaches into the penthouse suite at the SAP Center, Suite P10. 5-step sequence.

---

**Sequence at a Glance**

| Step | Type | Timing | Goal |
|---|---|---|---|
| Email 1 | ✋ MANUAL | 3–4 weeks out | Initial invite — are you going? Book suite time. |
| Call 1 | ✋ MANUAL | 2–3 days after Email 1 | Confirm attendance; book directly on the call. |
| Email 2 | ⚡ AUTO | 2 weeks out | Show what we're building; give them a reason to come. |
| Call 2 | ✋ MANUAL | 10–14 days out | Final push — book on the call or pivot to post-Games. |
| Email 3 | ⚡ AUTO | 1 week out | Last chance; graceful pivot if not attending. |

---

**Email 1 — The Initial Invite**
Send: 3–4 weeks before July 24 | ✋ MANUAL | 🧪 MOPS TEST REQUIRED

*Before sending: review any prior conversation notes and add relevant context to personalize. This email comes from the rep, not a marketing alias.*

🧪 MOPS: Send a test of "Email 1 — The Initial Invite" before deploying. Confirm subject line, preview text, all `{tokens}` render correctly, send-from address shows rep name, and timing trigger fires as expected.

```
From: {Rep First Name} <{rep@sugarwod.com}>
To: SugarWOD CrossFit customer or warm prospect
Subject: Are you heading to the CrossFit Games?
Preview: We have a suite at the SAP Center. Would love to have you.
```

Hey {First Name},

Are you planning to be in San Jose for the CrossFit Games this year?

We're hosting a penthouse suite at the SAP Center for Games week (July 24–26) and I'd love to have you join us. VIP access above the floor, food and drinks, and a gift bag waiting when you arrive. Good people, great competition.

I'd also love to catch up on what's going on at {Gym Name} and share a few things we've been working on. Can I put you down for a time while you're in town?

Just reply and let me know if you're going and I'll get you on the calendar.

Hope to see you there,
{Rep First Name}

*Personalization notes: For existing customers, reference something specific to their account or a recent conversation. For prospects, keep focus on the Games experience — save product detail for the suite.*

---

**Call 1 — The Follow-Up**
Timing: 2–3 days after Email 1 if no reply | ✋ MANUAL
Fallback: Voicemail below, then move to Email 2

**If They Answer:**

Hey {First Name}, it's {Rep Name} from SugarWOD. Do you have a quick minute? [ WAIT ]

I sent you a note a few days ago about the CrossFit Games. We're hosting a suite at the SAP Center and I wanted to make sure you got the invite. Are you planning to be in San Jose?

**IF ATTENDING — Book on the call:**
Perfect. I have my calendar open right now. We're there July 24, 25, and 26. What day works best for you? [ WAIT ] Great. Morning or afternoon? [ LOCK IN THE TIME. Confirm out loud. ] I'll put you down for {Day} at {Time} in Suite P10 at the SAP Center. I'll send you a calendar hold with the details.

📅 *Send calendar invite immediately after the call. Include: SAP Center, Suite P10, San Jose, arrival instructions.*

**After booking:** "When you come through we'll catch up on what's going on at {Gym Name} and I'll walk you through a few things we've been building. Should be a good conversation." *Keep it light — detail comes in the suite, not on this call.*

**IF NOT ATTENDING:** No worries. We'll also be at the Owners Conference on July 22–23 at the Signia if that's easier. And if you're not making the trip this year, I'd love to find 20 minutes before the summer gets away from us. What does your calendar look like in the next couple of weeks? [ Book a call directly. Don't leave it open. ]

**Objection Handling:**
- *"My schedule is packed that week."* → I get it. Even 30 minutes is worth it. What's the least busy day for you? I'll work around whatever you've got.
- *"We're happy with SugarWOD right now."* → That's good to hear. I still want to show you a few things we've been building that I think are worth your time. Come watch the Games and we'll find a few minutes while you're there.
- *"We're looking at other options."* → Then let's make sure you have the full picture before you decide. Come through the suite and we'll talk it through.

**Voicemail:**
Hey {First Name}, it's {Rep Name} from SugarWOD. I sent you a note a few days ago about the CrossFit Games. We're hosting a suite at the SAP Center and I have a spot for you. Give me a call back at {Rep Phone Number} and I'll get you on the calendar. Talk soon.

---

**Email 2 — What We're Building**
Send: 2 weeks before July 24 | ⚡ AUTOMATED | 🧪 MOPS TEST REQUIRED
Trigger: 14 days before July 24 AND no booking logged for contact

🧪 MOPS: Send a test of "Email 2 — What We're Building." Confirm subject line, preview text, all `{tokens}` render correctly, send-from address shows rep name, and timing trigger fires as expected.

```
From: {Rep First Name} <{rep@sugarwod.com}> (send-from mapped to assigned rep)
To: Anyone in sequence who has not booked after Email 1 + Call 1
Subject: What we're showing at the Games this year
Preview: A few things worth your time while you're in San Jose.
```

Hey {First Name},

We're two weeks out and I wanted to give you a look at what we'll be covering in the suite this year.

- **The programming marketplace:** Expert programming published directly to your SugarWOD calendar. Your athletes get vetted programming from coaches who know CrossFit and you spend less time managing it.
- **Leaderboards and PR tracking:** Members who track their progress and compete with their community stay longer. I have some data on this that's worth seeing.
- **The full Games week picture:** We're also at the Owners Conference on July 22–23 and sponsoring the Adaptive CrossFit Games. If any of those are relevant, I can connect you with the right people while we're all in the same place.

Are you going to be in San Jose? Reply and I'll get you on the calendar for a time in the suite.

{Rep First Name}

*Personalization notes: Adjust product bullets to match what's most relevant to this contact. If prospect (not yet a customer), consider swapping one bullet for something community/experience-forward.*

---

**Call 2 — The Final Push**
Timing: 10–14 days before July 24 | ✋ MANUAL
Fallback: Voicemail below, then move to Email 3

**If They Answer:**

Hey {First Name}, it's {Rep Name}. Quick follow-up on the Games suite. We're about two weeks out and I want to make sure I have you on the calendar before it fills up. Are you going to San Jose?

**IF YES:** What day works best for you? I have my calendar open right now. [ BOOK IT ON THE CALL. Confirm day and time. Send invite immediately after. ]

**IF NO — Pivot immediately:** Got it. Can we find 20 minutes before the end of July to catch up instead? I want to show you what we've been building and hear what's going on at {Gym Name}. What does your week look like? [ BOOK A CALL. Do not leave it open. ]

**Objection Handling:**
- *"I need to check my schedule."* → What day is looking lighter? I can work around most things. Even 30 minutes is worth the trip up to the suite.
- *"I don't think I'm going this year."* → No problem. When's a good time to connect before the summer? I want to make sure we have a chance to talk through a few things.
- *"Just send me the info."* → I'd rather just grab 5 minutes now and put something on the calendar while I have you. What day works?

**Voicemail:**
Hey {First Name}, {Rep Name} from SugarWOD. Following up on the Games suite one more time. We're two weeks out and I want to get you on the calendar. Call me back at {Rep Phone Number} and I'll book you in. Otherwise I'll try you again before the week starts.

---

**Email 3 — Last Chance**
Send: 1 week before July 22 | ⚡ AUTOMATED | 🧪 MOPS TEST REQUIRED
Trigger: 7 days before July 22 AND no booking logged for contact

🧪 MOPS: Send a test of "Email 3 — Last Chance." Confirm subject line, preview text, all `{tokens}` render correctly, send-from address shows rep name, and timing trigger fires as expected.

```
From: {Rep First Name} <{rep@sugarwod.com}> (send-from mapped to assigned rep)
Subject: One week out: a few spots left
Preview: If you're heading to San Jose, reply and I'll get you on the calendar.
```

Hey {First Name},

Games week is one week away. I still have a couple of open spots in the suite and wanted to check in one more time.

Here's the full picture of what we're doing:
- CrossFit Owners and Coaches Conference · July 22–23 at the Signia by Hilton. We'll be at our booth.
- CrossFit Games · July 24–26 at the SAP Center. Penthouse suite above the floor. Food, drinks, and gift bags when you arrive.
- Adaptive CrossFit Games · July 24–26 at the San Jose Convention Center. Presented by WheelWOD. We're proud to be a sponsor and will have a team there all three days.

If you're going to be in San Jose, just reply and I'll get you on the calendar. Takes two minutes.

And if you're not making the trip this year, let's find time after the summer. Just reply and we'll figure something out.

{Rep First Name}

---

**Token Reference**

| Token | Meaning | Used In |
|---|---|---|
| {First Name} | Contact's first name | All emails, all calls |
| {Rep First Name} | Rep's first name | Email sign-offs |
| {rep@sugarwod.com} | Rep's work email address | From address |
| {Rep Name} | Rep's full name | Call openings, voicemails |
| {Rep Phone Number} | Rep's direct phone number | Voicemails |
| {Gym Name} | Contact's gym or business name | All touchpoints |
| {Day} | Booked day (e.g., Friday July 25) | Call 1 & 2 booking confirmation |
| {Time} | Booked time (e.g., 2:00 PM) | Call 1 & 2 booking confirmation |

---

> **📋 MOPs Checklist — Before This Sequence Goes Live:**
> - [ ] Review send type on each step (Emails 1 + manual calls = Manual; Emails 2 + 3 = Automated — confirm triggers)
> - [ ] Send a test of Email 2 and Email 3; confirm formatting, links, and all `{tokens}` render correctly
> - [ ] Confirm send-from address on automated emails maps to the correct rep
> - [ ] Review all copy against Boutique / SugarWOD voice standards
> - [ ] Confirm all `{tokens}` are either pre-populated or flagged for rep
> - [ ] QA trigger conditions for Email 2 (14 days pre-event, no booking) and Email 3 (7 days pre-event, no booking)

---

## Example B: CFG 2026 Post-Event Sequence (Boutique / SugarWOD)

**Context:** Post-event follow-up for anyone with a meaningful interaction during Games week. Goal: book a follow-up call. 5-step sequence.

---

**Sequence at a Glance**

| Step | Type | Timing | Goal |
|---|---|---|---|
| Email 1 | ✋ MANUAL | 1–2 days post-event | Warm, specific follow-up — ask for a call. |
| Call 1 | ✋ MANUAL | 3–5 days post-event | Reference the conversation. Book the call. |
| Email 2 | ⚡ AUTO | 1 week post-event | Give them a reason to respond. |
| Call 2 | ✋ MANUAL | 10–12 days post-event | Direct check-in — book it or find out what's in the way. |
| Email 3 | ⚡ AUTO | 2–3 weeks post-event | Low-pressure close. Leaves the door open. Ends the sequence. |

---

**Email 1 — The Day-After Follow-Up**
Send: 1–2 days after Games week ends | ✋ MANUAL

*Before sending: review Popl notes or any conversation notes and write in the specific detail for `{One specific thing from the conversation}`. A generic follow-up after a personal interaction wastes the relationship just built.*

📋 Rep tip: Write one real thing you remember from your conversation with this person. Use it. Check Popl notes if needed.

```
From: {Rep First Name} <{rep@sugarwod.com}>
Subject: Great meeting you in San Jose
Preview: Wanted to follow up while it's still fresh.
```

Hey {First Name},

Really glad we got to connect in San Jose. {One specific thing from the conversation — e.g. "What you said about retention dropping in the summer really stuck with me" or "Sounds like you have a strong community at {Gym Name} and I'd love to help you keep it that way."}

I want to make sure we actually follow through on what we talked about. Can we find 20–30 minutes in the next week or two to pick up where we left off?

What does your calendar look like? I'll work around you.

{Rep First Name}

*`{One specific thing from the conversation}` is not optional. Write something real. If you can't remember, check your Popl notes before sending.*

---

**Call 1, Email 2, Call 2, Email 3** follow the same structure as the pre-event sequence above. See CFG 2026 Post-Event Sequence document for full call scripts, objection handling, voicemails, and automated email body copy.

Key differences in post-event tone:
- Opens by referencing the specific interaction ("what you said about X") not the event itself
- Goal shifts from "come to the suite" to "book a follow-up call"
- Email 3 is a clean exit — respects their time, sets up re-engagement later in the year

---

**Token Reference (Post-Event)**

| Token | Meaning | Used In |
|---|---|---|
| {First Name} | Contact's first name | All emails, all calls |
| {Rep First Name} | Rep's first name | Email sign-offs |
| {rep@sugarwod.com} | Rep's work email | From address |
| {Rep Name} | Rep's full name | Call openings, voicemails |
| {Rep Phone Number} | Rep's direct phone number | Voicemails |
| {Gym Name} | Contact's gym name | All touchpoints |
| {One specific thing from the conversation} | Real detail from Games week — written by rep before send | Email 1, Call 1 |
| {Reference the specific thing} | Callback to their pain point or topic | Call 1 script |

---

## Example C: HFA 2026 Sales Talk Track + Meetings Process (Enterprise / Club Automation — Tier 1)

**Context:** Tier 1 event. Large pre-scheduled meeting push. Three meeting types (Customer, Strategic Prospect, Cold/BDR). Separate talk track and booking process documents generated alongside the sequence.

### Talk Track Format

Each audience type gets its own call script with:
- Opening (personalized to relationship type)
- Meeting pitch (outcome-focused, not feature list)
- If YES: booking confirmation + next steps
- If NO: graceful exit + offer for virtual follow-up or booth drop-in

**Customer Opening:**
Hi {first_name}, I hope you're doing well. Are you planning to attend HFA 2026 this year? If so, I'd love to meet with you during the conference to learn more about how things are going at your club and how you're currently using Daxko — specifically {product(s) they use}. It's a great opportunity to talk through what's working well today and explore how you can go all in on smarter operations...

**Strategic Prospect Opening:**
Hi {first_name}, how are you? Since you and your team are already exploring Daxko's solutions, I wanted to invite you to connect with us in person at HFA 2026. Meeting during the show gives us a chance to walk through AI-first workflows and real operational use cases, show how clubs are removing friction across the member journey...

**BDR (Landing Page Inbound) Opening:**
Hi {first_name}, how are you today? I saw that you're interested in meeting with us at HFA 2026, and I wanted to connect to get that scheduled. During our time together, we can walk through AI-first workflows, share examples of how clubs like yours improve engagement, retention, and payments...

### Post-Conversation Steps (all meeting types)
1. Send booking link
2. Forward Outlook invite to relevant internal team / ELT
3. Complete meeting brief and share with attendees
4. Confirmation email sends automatically

### Adding ELT/Product/Services
- Email Stephen Deperty with request to add ELT/Product/Services
- After approval: forward the meeting invitation to the necessary team members
- Khang, Adam, and/or Wes (TBD on who is attending) can be booked together or separately

---

## Writing Notes

- **Book on the call.** Every call script reminds the rep: get a specific day and time, confirm out loud, send the calendar invite immediately. Never leave a call with "I'll send you a link."
- **Post-event Email 1 is the highest-priority touchpoint.** It must be specific. Generic post-event follow-ups are wasted sends. The `{One specific thing from the conversation}` token is mandatory, not optional.
- **Automated emails still map to the rep's address.** Replies land with the rep, not a marketing inbox. Note this explicitly in every automated step.
- **Token tables are required.** Every sequence ends with a complete token reference, no exceptions.
- **Tier 1 events get a separate meetings process doc.** Ask the user to confirm before generating.
