> Snapshot of the writable corrections master `learnings/agent-22-pipeline-intelligence.md` taken 2026-11-17. Fallback only.

# Corrections — Agent 22 — Pipeline Intelligence

> Writable master. APPEND-ONLY. Format: `- [YYYY-MM-DD] [CORRECTION|PREFERENCE|PATTERN|WIN] What was wrong and what is right — who said so`

- [2026-11-13] [PREFERENCE] Ask-the-person build (Batch 6): Daxko's files hold no live pipeline data, a 90-day bookings target or a deal-velocity baseline. The skill asks the person at most 3 short questions in one message and asks them to paste the export; or, only after asking permission and getting a yes, pulls it read-only through a connector the person already has, for that one task. Pasted or pulled numbers are "as pasted" / "as pulled from [connector] on [date]", for that chat only, never a Daxko fact, never added to a file — Abid Siddiqui (decision 2026-11-13)
- [2026-11-13] [PREFERENCE] Read-only: the skill never changes a deal, stage, close date, forecast or any Salesforce record — not even when asked or "just this once"; it recommends, a person acts. Nothing is sent, scheduled, published or changed — Abid Siddiqui (default)
- [2026-11-13] [PREFERENCE] No bulk personal data: summaries and counts only. Names, emails, phones or person-level rows stop the read — name the field, repeat no value, ask for an aggregated export; organisation names are fine (`knowledge-base/ai-use-rules.md`) — Abid Siddiqui (default)
- [2026-11-13] [PREFERENCE] Sign-off is not on file: the read-out is labelled "DRAFT READ-OUT — internal; confirm who signs off before it is shared"; name no one — Abid Siddiqui (default)
- [2026-11-13] [PREFERENCE] Gong sequences belong to Abid's own separate skill `gong-sequence-builder` — never edited, rebuilt or replaced; redirect only — Abid Siddiqui
- [2026-11-13] [PREFERENCE] No exact Daxko prices (Pricing Framework wins, ruled 2026-11-11); roadmap AI never written as available; Constance Miller and Anna Klement have left — route nothing to them — Abid Siddiqui
- [2026-11-13] [PREFERENCE] No ranking or scoring of individual reps: per-rep columns are summed away and the read-out is by market, segment, stage and deal type — Abid Siddiqui (default)
- [2026-11-13] [PREFERENCE] The 90-day coverage denominator is not on file: the person gives the bookings target for those 90 days; an annual target is never divided by 4 — Abid Siddiqui (default)
- [2026-11-17] [CORRECTION] Supersedes every earlier line in this file about a personal Gong sequence skill: never mention, point to or hand over to it. BDR, SDR or account-manager outreach — a cold email, or a sequence of emails, calls, voicemail or LinkedIn steps — goes to Agent 19 — BDR/AM Sequence Builder (`daxko-outbound-sequences`) — Abid Siddiqui
