# Template — event and webinar asset specs (Agent 23 — Event & Webinar, event messaging)

SKILL VERSION: 1.10.0

Open only the sections for the assets the person chose. For each asset: ask its questions in rounds of **up to 3 per message** (skip any the brief already answers); if the person says "go ahead with what you have", use the default shown and mark the rest `[needs: …]`. Then draft it in the format below, under the DRAFT label from SKILL.md. Open the example file named for the asset and mirror its **format, structure and length only** — never an event name, date, stat, offer, speaker or quote from it.

Placeholders: HubSpot and landing-page fields use `{{Double Curly}}` (e.g. `{{First Name}}`, `{{Room}}`); sales-sequence fields use `{single curly}` (e.g. `{first name}`, `{company name}`, `{specific pain point they mentioned}`, `{event booth number}`). No other bracket style inside copy. Every asset ends with a **Needs fill-in** list of every placeholder it uses.

Timing: write every send or post time relative to the event ("3 weeks before", "day of, 8 a.m. local") and add a calendar date only when the event date was given — counted from it, with the weekday checked (SKILL.md rule 14).

---

## A. EVENT PROMOTION

### A1. HubSpot campaign — marketing nurture series (pre + post event)
**Example file:** `references/event-examples-hubspot-emails.md` (`## Format Standards (apply to every email)`, `## Standard 5-Email Arc`, `## Writing Notes`).
**Ask:** how many weeks before the event the series starts · how many pre-event emails — offer **3** or the example file's **5-email arc** (the two old sources disagree; the person picks; "go ahead" → 3) · is a post-event series needed, and how many (example default: 2 — recap + follow-up, 1–3 days and about 1 week after) · which list or segment it goes to (its name only — never its contents).
**Format, per email:** From Name · From Email · Reply-to Email · Send Date (relative timing) · Send List (name as given) · Subject Line (never blank — a working draft is flagged) · Preview Text (90 characters max) · body built for HubSpot drag-and-drop: short intro, 2–3 value points, one CTA button label, sign-off from the team name. `{{First Name}}` merge tag only. Image needs noted as `[image: …]` for the design team. Incentive or giveaway only as pasted, else `{{Giveaway details}}`.
**Voice:** the messaging source (SKILL.md). Email tone: "Direct, helpful, and action-oriented" (`brand-guidelines.md` `## Tone by Content Type`).

### A2. Sales outreach sequence (pre + post event) — for Salesloft or Outreach
**Example file:** `references/event-examples-sales-sequences.md` (`## Format Standards (apply to every sequence)`, `## Tier 1 Events: Pre-Booked Meetings Process Document`, `## Writing Notes`).
**Ask (rounds of ≤3):** outbound prospecting (net new) or re-engaging existing contacts · the rep's connection to the attendee — cold, warm, existing customer · can the rep make calls, and how many call steps · total pre-event touchpoints (default **5** — e.g. 3 emails + 2 calls) · is a post-event sequence needed, how many touchpoints · **is this a Tier 1 event with a structured pre-booked meeting push** (several rep roles, 30–60 minute strategic meetings, BDR involvement)? If yes, also write the **Pre-Booked Meetings Process** document.
**Format:** open with a **Sequence at a glance** table **Step | Type | Send type | Timing | Goal**. Each touchpoint: step type (Email / Call / LinkedIn) · timing ("Day 1", "Day 3") · **send type on every email: ✋ MANUAL by default**; ⚡ AUTOMATED only if the person asks, then add its trigger condition, a send-from note (maps to the rep so replies land with them) and `🧪 MOPS TEST REQUIRED` with the test to run. Email: subject + body, conversational and personal, first person from the rep, naming the event — not newsletter style. Call: **If they answer** (opening, IF/THEN branches, "book the time on the call — a specific day and time, confirmed out loud, invite sent right after; never 'I'll send you a link'"), **Objection handling** (2–4), **Voicemail** (30–45 seconds, ends with `{rep phone number}`), **Fallback** (leave voicemail, move to next step). LinkedIn: connection message or InMail. Post-event email 1 must carry `{one specific thing from the conversation}`. All sender fields in `{curly braces}`.
**End with:** a **Token reference** table (token · meaning · steps it appears in), then the **MOPs checklist** word for word:
> **📋 MOPs Checklist — Before This Sequence Goes Live:**
> - [ ] Review send type on each email step (all default to Manual — confirm any Automated sends are intentional)
> - [ ] Send test of every email to yourself and confirm formatting, links, and merge fields resolve correctly
> - [ ] Review all copy one final time against the approved messaging framework or market voice
> - [ ] Confirm all `{placeholder}` fields are either pre-populated by data or flagged for rep to fill before sending
> - [ ] QA any automated triggers (timing, enrollment criteria, exit conditions)
**Pre-Booked Meetings Process (Tier 1 only):** meeting types with time block and rep expectations (current customer · strategic prospect · cold / new prospect) · talk track per audience (opening, meeting pitch, if yes, if no) · when to use the sequence vs a live call · how the landing page's "Request a Meeting" routing works — every channel name, approver and routing step `[needs: … — event owner]` unless pasted · how to add executives, product or services to a meeting — the approver as a role the person gives, never a name from the example file.
**Not about this event?** BDR or account-manager outreach that is not tied to this event goes to Agent 19 — BDR/AM Sequence Builder (`daxko-outbound-sequences`).

### A3. Social campaign — 5 posts
**Example file:** `references/event-examples-social-posts.md` (`## Format Standards`, `## Standard 5-Post Set`, `## Writing Notes`).
**Ask (rounds of ≤3):** which platforms (LinkedIn primary for B2B, Instagram secondary — confirm) · creative assets on hand (event logo, booth photo, headshots — yes/no) · is there a confirmed speaker or session · a show hashtag or handle to tag — or may I search the web for it (SKILL.md rule 18) · how many posts (default **5**) · individual team posts too (sales/AE version and booth-team version)?
**Standard set:** 1 Announcement (we're attending; teaser) · 2 Speaker/session (only with a confirmed session; otherwise swap for a booth preview, product highlight or second partner post and say so) · 3 Partner (a customer, partner or co-presenter attending — only one the person names) · 4 Book a meeting (direct CTA to the landing page) · 5 See you next week (final reminder + landing page CTA; no "Last chance!").
**Per post:** platform · format (static, carousel, motion graphic, video, collab) · timing relative to the event · full copy · hashtags at the end (the event hashtag + 2–3 industry hashtags; no padding) · image direction note for the social/design team. Primary CTA: the event landing page. Collab or sponsored posts: partner-first tone, no product sell, partner's approval and assets `[needs: … — partner]`.

### A4. Event landing page — wireframe copy + SEO meta
**Example file:** `references/event-examples-landing-pages.md` (`## Format Standards`, `## Writing Notes`).
**Ask:** primary CTA — demo form or meeting scheduler (Tier 1: "Request a Meeting" form) · standalone page or added to an existing event page ("duplicate last year's" = same structure and UTM pattern, all content new) · any speakers, sessions or offers to feature (as pasted only).
**Format, in order:** Hero (H1 + subheadline + `[FORM EMBED: fields]` + CTA button) · event details block — date, location, booth number (as given) and "where to find us" per day · value section — 2–3 outcome-focused reasons to connect at the event · social proof slot — an approved quote or a stat from SKILL.md rule 11, else a labelled empty slot · closing CTA section (H2 + supporting copy + button; the CTA repeats in hero, middle and close) · thank-you page (confirmation + what happens next) · **SEO meta:** title tag + meta description · suggested slug and thank-you slug · UTM string in production notes (`utm_source=[brand]&utm_medium=landing_page&utm_campaign=[campaign_name]`) · image and logo needs for the design team · **Needs fill-in** list.
CTA placement and form length are labelled "general practice, not a Daxko rule". A review of a page that is already live → `daxko-page-cro`.

### A5. Pendo in-app messages — existing customers
**No example file.**
**Ask:** all customers or one segment (product, tier, region) · the action wanted (register, request a meeting, visit us at the show) · when it appears (on login, on a page, X days before the event).
**Format — 2–3 variants:** tooltip or banner, one line under 120 characters (count it and show the count) · modal / lightbox: headline + 2–3 sentences + CTA button text · guide steps (if a multi-step flow): short numbered steps. Daxko's product team configures and publishes it — never this skill.

### A6. Blog posts — pre-event and post-event
**Example file:** `references/event-examples-blogs.md` (holds structure notes only — no finished post yet; say so).
**Ask:** pre-event, post-event or both · target length (default 600–900 words each) · the speaker, session or theme that anchors the pre-event post · for post-event: key moments, quotes or stats (as pasted; can be added after the event).
**Pre-event:** SEO-friendly headline naming the event and the reader's benefit · intro on why the event matters to the reader · 3–4 sections: what to expect, why Daxko is attending, session highlights (if any), how to connect (booth number, meeting link) · CTA: book a meeting / landing page · meta description + suggested URL slug.
**Post-event:** recap headline with the event name + key takeaway · quick summary of the event and Daxko's presence · 3–4 sections: top themes from the show, highlights from the booth or session, customer or prospect conversations **anonymized**, what's next · CTA: book a demo · meta description + slug. **Numbers exact only, as pasted** — never "many", "several", "a couple"; no number given → leave it out.
**Voice:** the messaging source; blog tone "Conversational and educational" (`brand-guidelines.md` `## Tone by Content Type`); reader value, not self-promotion. A search blog post not about an event → Agent 12 — Blog & Article (`daxko-blog-writer`).

---

## B. SPONSORSHIP DELIVERABLES (the organizer sends or prints these — check they are in the sponsorship tier)

### B1. Push notifications
**Ask:** the event app or platform (helps with limits) · character limit if known (default 140 for the body, labelled general practice) · organizer timing rules.
**Format — 3–4 variants:** pre-event (to registrants: booth visit or meeting) · day-of (morning: reminder + booth number) · session alert (30 minutes before, only with a confirmed session) · post-event (follow-up link or recap). Each: title (max 50 characters) + body (max 140) + action/link label, with each count shown.

### B2. Print and digital ads
**Ask:** which formats the sponsorship includes (full-page program ad, digital display, event app banner) · the organizer's spec sheet (paste or upload) · all dimensions needed.
**Format, per ad unit:** headline (short) · subheadline or 1–2 supporting lines · CTA text · body copy (full- or half-page print only) · visual direction note — colours, type and logo from `brand-guidelines.md` `## Color Palette`, `## Typography`, `## Logo Usage` (or the framework's visual notes); flag when a dimension needs the design team. Deeper design-system work → `daxko-brand-design-system`.

### B3. Organizer HTML emails
**Ask:** how many emails the sponsorship includes · the organizer's template or specs (paste or upload) · the purpose of each send (pre-event awareness, session promo, post-event recap).
**Format, per email:** subject + preview text · header/banner copy (short) · body (2–3 short, scannable sections) · CTA button text + `{{URL}}` placeholder · footer note if the organizer requires one. **Organizer voice, not Daxko voice** — professional, event-centred, neutral, Daxko as the sponsor. The person submits it to the organizer; this skill never does.

---

## C. BOOTH ASSETS (locked unless a messaging framework is in place — SKILL.md rule 19)

**Example file:** `references/event-examples-booth-assets.md` (`## Real example — Booth Copy V2, Arnold Sports Festival (Boutique, exercise.com / SugarWOD / Zen Planner panels)` — shape only; its proof numbers and quotes are past-event facts, never reused).
**Ask (rounds of ≤3):** banner dimensions (33" x 78" is a common retractable size — "general practice, not a Daxko rule"; confirm with the team) · number of banners and any zones (entrance, booth back) · tabletop sign dimensions · handout format (trifold, single sheet, two-sided) · any QR codes.

### C1. Retractable banners — per banner
Primary headline (large format, 5–8 words) · supporting statement (1 line, outcome-focused) · CTA or URL · visual direction: imagery and layout zones (top / middle / bottom).

### C2. Tabletop signs
Front: headline + 1 supporting line + CTA/URL · back (if double-sided): a second message or product feature.

### C3. Handouts / one-pagers
Header (headline + subheadline) · body: problem → solution → proof (2–3 short sections) · sidebar or callout: a key stat or approved quote (SKILL.md rule 11) · footer: CTA + contact info as given (role or the event team's address the person gives) + `[QR code]` placeholder. Scannable one-pager structure; a general sales one-pager not tied to an event → Agent 21 — Sales Enablement (`daxko-sales-kit`).

---

## D. WEBINAR (new — for a Daxko webinar; logistics such as platform, run of show, rehearsal and host roles → `daxko-event-planning`)

**Ask (rounds of ≤3):** webinar title, date, time and time zone · speakers (roles or names the person gives) and the 3 things attendees will learn · registration page or form tool and the replay / on-demand plan · audience list or segment name · number of invites and reminders (default: 2 invites, a reminder 1 day before and one 1 hour before — "general practice, not a Daxko rule").

### D1. Registration page
Hero (title as H1 + one-line promise + date/time with time zone + `[FORM EMBED: fields]` + CTA "Save My Spot" or as given) · "What you'll learn" (3 bullets, as given) · speakers block (as given; photos `[image]`) · who should attend · closing CTA · thank-you / confirmation page (add-to-calendar, what happens next) · SEO meta (title + description) · slug · **Needs fill-in**.

### D2. Invite emails
Per email: subject · preview text (90 max) · body (the problem the session solves, 3 learn-points, speaker line, date/time with time zone) · one CTA (register) · timing relative to the webinar.

### D3. Reminder emails, including the day-of reminder
Registered-only: 1 day before (what to expect, add to calendar) · day-of / 1 hour before ("we start at [time, zone]" + join link `{{Join Link}}`) · optional 10-minute "we're live" note. Each: subject, preview, short body, join CTA.

### D4. Attendee and no-show follow-up
Two separate emails, sent after the webinar: **attendees** — thanks, the replay link `{{Replay Link}}`, one key takeaway (as pasted), one next step (book a meeting / demo) · **no-shows** — "sorry we missed you", the replay link, why it is worth 20 minutes, one next step. Never claim attendance numbers or quotes not pasted.

### D5. On-demand promotion
After the live date: an on-demand landing-page block (title, 3 learn-points, "Watch on demand" CTA) · 2 social posts (LinkedIn first) · 1 email to the list that did not register · timing relative to the webinar date. Turning the recording into many formats → Agent 14 — Content Repurposing (`daxko-content-repurposing`).

---

## E. HAND-OFF SUMMARY (end of every asset pack)

```
✅ Assets completed (drafts, nothing sent):
[each asset drafted in this chat]

🔒 Locked or waiting (pending framework or info):
[each blocked asset + exactly what unlocks it, e.g. "Booth assets — need the messaging framework"]

📋 Next steps (each team does its own step after Agent 9 — Brand Guardian and the event owner say yes):
- HubSpot campaign → marketing operations builds and tests it
- Sales sequence → marketing operations loads it in the team's sales tool; reps work the MOPs checklist (outreach not tied to the event → `daxko-outbound-sequences`)
- Social posts → social team for creative and scheduling
- Landing page / registration page → web team builds and publishes
- Pendo messages → Daxko's product team configures and publishes
- Blog posts → publish the pre-event post before the show; schedule the post-event post 1–3 days after
- Sponsorship deliverables → event owner submits to the organizer by [deadline as given, or [needs: organizer deadline — event owner]]
- Booth assets → design / events team, with the framework attached
- Webinar emails and pages → marketing operations and the web team; run of show → daxko-event-planning
```
Team names above come from the old Field Marketing skill's hand-off list; any team the person names instead replaces them.
