# Agent 23 — Event & Webinar (event messaging) — teammate guide

**Skill:** `daxko-event-promotion` · **Owner:** Abid Siddiqui · **Version:** 1.10.1

## What it does
For ONE Daxko event or webinar, it writes the promotion copy: pre- and post-event HubSpot emails, a sales outreach sequence (emails, calls, LinkedIn), 5 social posts, the event landing page, Pendo in-app messages, pre- and post-event blogs, sponsor pieces (push notifications, ads, organizer emails), booth copy (banners, table signs, handouts) and webinar pieces (registration page, invites, reminders, follow-up for attendees and no-shows, on-demand promotion). It asks about your messaging framework first, then the event brief, your main call to action and what you are promoting, then shows a menu to pick from. It asks up to 3 questions at a time and uses only what you paste. It is the upgraded version of Field Marketing's old `daxko-event-comms` skill.

## Requests to try
- "Event assets for NAYDO — emails, sales sequence and social"
- "Webinar invite and reminder emails for our Club Automation payments webinar"
- "Booth banner and table sign copy for HFA — framework attached"

## What it may change, and only after your yes
If you have a connector, it can save **unsent draft** emails in HubSpot, **inactive** draft sequence steps (no contacts) in Salesloft or Outreach, or one Asana task or document with the asset pack. It first shows you the exact list and waits for your "yes" in the chat. You become the owner of that change.

## What it never does
Send or schedule an email, add contacts to a sequence, turn a sequence on, publish a page, blog or in-app message, schedule or post on social, send anything to the event organizer, or delete anything. It never invents stats, quotes, speakers, offers, hashtags or dates.

## What it will NOT do — and who does
| Ask | Owner |
|---|---|
| Event logistics, travel, workback schedule, webinar run of show, post-event recap and ROI score | `daxko-event-planning` (Agent 23 — Event & Webinar, event planning) |
| An email nurture not tied to an event | Agent 15 — Email & Nurture |
| A launch kit not tied to an event | Agent 13 — Content Production |
| An outreach sequence | `daxko-outbound-sequences` |
| Brand check before anything goes out | Agent 9 — Brand Guardian |
