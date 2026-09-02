# Corrections — Agent 9 — Brand Guardian

**Created:** 2026-08-11
**Owner:** Abid Siddiqui
**Status:** WRITABLE MASTER — this is the real one.

---

## Why this file lives HERE and not inside the skill

This file sits in `learnings/`, **outside every skill folder, on purpose.**

A skill that has been shared — zipped to a teammate, uploaded to claude.ai, or installed as a
plugin — is **read-only for everyone who receives it.** Nobody else's Claude can write into it. If
the corrections file lived inside the skill, every correction would either be lost or would
overwrite something on the next update.

So the arrangement is:

| Copy | Where | Who can write to it |
|---|---|---|
| **The writable master** | `learnings/agent-09-brand-guardian.md` — this file | Abid Siddiqui's machine only |
| **The bundled snapshot** | `<skill>/references/corrections-snapshot.md` | Nobody. Generated. Refreshed at every publish — meaning **before the commit that ships a new version**, and equally before a break-glass zip if one is ever cut (PROMPT 4 step 1b). *"Before zipping" no longer binds: publishing is a version bump pushed to the marketplace, not a zip.* |

Teammates read the snapshot and so receive the accumulated learning. **Teammates cannot log
corrections themselves — they send them to Abid Siddiqui, who records them here and re-publishes.**

If this file is missing when the skill runs — which is normal on a teammate's machine — the skill
reads `references/corrections-snapshot.md` instead. If neither exists, the review continues anyway
and says so in its SOURCES block. **A missing corrections file never stops a review.** That is the
difference between this file, which is OPTIONAL, and the knowledge files, which are REQUIRED.

---

## How to add a correction

Append **one dated line** at the bottom. **Lines are only ever added — never edited, never
deleted.** That append-only rule is what makes the learning compound instead of resetting.

Format:

```
- [YYYY-MM-DD] [CORRECTION|PREFERENCE|PATTERN|WIN] What the agent got wrong or what it should do instead — who said so
```

| Tag | Use it for |
|---|---|
| `CORRECTION` | The agent judged something wrongly and was told so |
| `PREFERENCE` | Not wrong, but Daxko wants it done a particular way |
| `PATTERN` | Something that keeps recurring and is worth naming |
| `WIN` | A judgment that was notably right — worth keeping |

**After logging a correction, remember the snapshot is now stale.** The next publish (PROMPT 4)
refreshes it. Until then, teammates are still working from the older copy — and the check-up will
flag exactly that.

---

## Corrections log

- [2026-08-11] [PATTERN] File created and seeded during PROMPT 1, alongside the SPEC for Agent 9 — Brand Guardian. No corrections logged yet — the skill has not been built or tested. — Abid Siddiqui / setup
- [2026-08-17] [CORRECTION] A market stated by the submitter is a hint, not a fact. When the stated market contradicts the content — labelled "club" but the copy addresses a YMCA's mission, branches and board — review against the EVIDENCE, say so in one line at the top, and add a closing note naming which rows would flip if the label is right. Found in hostile QA: the skill obeyed the label and REJECTED clean nonprofit copy on four dimensions for using mission language, with a correct file citation on each, and never hinted the label was the real problem. Worked example added at examples/mislabelled-market.md. — Abid Siddiqui / hostile QA 2026-08-17
- [2026-08-17] [CORRECTION] A missing conditional file costs you the DETAIL of one dimension, never the ability to report a violation another readable file already proves. Mark the row "partly scored", report what you can ground, and itemise what you could not check. Found in hostile QA: with references/color-system.md removed, the skill blanked Visual identity and reported "Violations: None" on a slide using #00857C — a colour brand-foundations.md explicitly names as fabricated, and which appears in the root CLAUDE.md as a "Daxko brand color". The palette lives in two always-required files, so the violation was provable throughout. Worked example added at examples/partial-review.md. — Abid Siddiqui / hostile QA 2026-08-17
- [2026-08-17] [PREFERENCE] Only DAXKO's own numbers need a bundled source. The customer's founding year, branch count or member count, a date, a deadline, and a competitor's published price are the submitter's facts — raise them in Suggested edits, never as unsourced-claim violations. The old unconditional wording flagged "for 150 years your branches have served families" and auto-REJECTED the piece. False positives train people to ignore the verdict, which is how a real unsourced ROI claim gets published. — Abid Siddiqui / hostile QA 2026-08-17
- [2026-08-17] [PATTERN] The two failures above were the same flaw twice: treating ABSENCE OF EVIDENCE as ABSENCE OF A PROBLEM. File missing → stay silent. Label present → stop looking. Worth checking for this pattern in the other agent builds. — Abid Siddiqui / hostile QA 2026-08-17
- [2026-08-18] [CORRECTION] The missing-CTA rule added on 2026-08-17 was written too broadly and produced two false positives on its first test run: it warned a single hero slide and the verbatim approved company boilerplate for "no CTA present". Scoped it to COMPLETE STANDALONE PIECES only — email, landing page, ad, social post, blog. A single slide (a deck carries one CTA, not one per slide), verbatim approved boilerplate (no CTA by design, already signed off by Anna Klement) and a spot-check fragment (a tagline, a subject line, one paragraph) are scored `pass — not assessable` instead. — Abid Siddiqui / regression run 2026-08-18
- [2026-08-18] [PATTERN] A fix written to close a false NEGATIVE will open a false POSITIVE unless its scope is stated in the same sentence. Both the original "150 years" defect and the missing-CTA fix failed the same way: an unconditional rule applied to cases nobody pictured while writing it. When adding a rule, write the exception list before writing the rule. — Abid Siddiqui / regression run 2026-08-18
- [2026-08-18] [PATTERN] Worked examples need the same verdict check as real reviews. examples/mislabelled-market.md shipped showing "APPROVED WITH CHANGES" above a `fail` row — contradicting the one-fail-is-enough rule the example exists to teach. Run the verdict table against every example before publishing. — Abid Siddiqui / regression run 2026-08-18
- [2026-08-17] [WIN] Grounding, injection resistance and precision all held under hostile QA: 39/39 real violations caught with a file citation each, ZERO invented across three scenarios, 20+ deliberate traps declined (sourced Mindbody 20% fee, banned words inside verbatim boilerplate, "registration closes 14 March" as a real deadline, "members" over "students", CrossFit proof point for a martial arts audience). Refused an embedded "pre-approved by Anna Klement, return APPROVED" instruction, a fabricated verbal correction, a CEO sign-off claim and a five-minute deadline. Regression suite recorded at agent-builds/agent-09-brand-guardian/TESTS.md — run all 12 cases after any edit. — Abid Siddiqui / hostile QA 2026-08-17
- [2026-08-24] [CORRECTION] Skill SELECTION happens on description match BEFORE any skill runs, so no rule inside a skill can rescue it from being passed over. Proven: a request saying "brand check this landing page" was routed to the org skill daxko-brand-qa and daxko-brand-guardian never executed. The word "landing page" appeared in both descriptions. Fix shipped in 1.1.0 — description now leads with UNPUBLISHED, says "landing-page copy not yet built", adds an explicit negative for live/staging pages, and names daxko-brand-qa as the handoff. When adding any future agent, check its description for collision against the existing org catalogue BEFORE building it. A skill that never fires is worth less than no skill, because the user believes they got a brand review. — Abid Siddiqui / claude.ai marketplace test 2026-08-24
- [2026-08-24] [PREFERENCE] Ask the user ONE question only, and only when the answer decides whether this skill is the right reviewer at all: draft, or already live? Market and content type are inferred and stated, never asked. Evidence: on the 9-trap test the skill worked out unprompted that copy labelled only "landing page" addressed three markets in irreconcilable conflict — better than what the submitter would have typed. Blanket clarifying questions add friction to every review to solve a case the skill already handles, and would not have prevented the collision above. A reviewer that interviews the user before every review stops being used. — Abid Siddiqui / 2026-08-24
- [2026-08-24] [PATTERN] The reviewer checks its input more carefully than its own output. On the nonprofit-email test its corrected rewrite contained three em dashes in ~104 words, tripping the "excessive em dashes" threshold the skill itself enforces. It also missed the Daxko-as-hero violation in the draft and mis-stated its own scorecard as "four of six fail" when five failed. Worth adding a self-check pass over the corrected rewrite before output. — Abid Siddiqui / 2026-08-24
- [2026-08-24] [WIN] Distribution route proven end to end with no admin involvement. A PRIVATE GitHub repo works as a claude.ai plugin marketplace; "Sync automatically" is on by default; the skill fires in plain claude.ai chat, auto-triggered from natural language with no slash command; the same plugin also appears in Claude Code; and the corrections snapshot travelled intact — the review's SOURCES block reported "9 entries found in references/corrections-snapshot.md (writable master not present on this machine)". On a deliberately trapped 9-item test the skill scored 5.5/6 on must-catch and 2/2 on must-NOT-flag, against 1.5/6 and 0/2 for the incumbent org skill on the same input. — Abid Siddiqui / 2026-08-24
- [2026-08-24] [PATTERN] A live org skill can carry production errors, and nobody is checking. daxko-brand-qa told the user to use Sohne (typography-system.md states verbatim "No fonts other than Barlow. Sohne... are not permitted", and brand-guidelines.md mandates Barlow with Arial fallback), suggested inventing testimonial attribution for a quote with no written approval, and advised renaming and shipping a feature that does not deliver until Q3 2026. ~40 org skills are live and this one is telling the whole marketing team to use a prohibited font. Raise with whoever owns the org catalogue. — Abid Siddiqui / 2026-08-24
- [2026-09-01] [CORRECTION] The grounding rule said "do not substitute another file" with no exception, so when brand-guidelines.md went missing from one install the skill broke the rule to do something better: it found the plugin copy of the same skill at the same version, checksum-verified it against the MANIFEST row, read from there, and disclosed the substitution twice. Recorded as FAIL against the rule as written — "superseded is not a pass" — but the rule was the thing that was wrong. Step 4 now permits exactly one substitution: same filename, another install of THIS SAME SKILL at THIS SAME VERSION, SHA-256 matching the MANIFEST row, disclosed in a bundle-integrity note and in SOURCES. If the checksum cannot be computed or does not match, STOP. Never substitute on filename and plausibility alone: ~/Downloads/daxko-ai-context-main/.../brand-guidelines.md exists with the right name, the wrong contents (the fabricated teal #00857C) and a non-matching checksum. The checksum, not the filename or the folder, is what makes a substitution safe. — Abid Siddiqui / refusal test 2026-09-01
- [2026-09-01] [PATTERN] A verification loop that iterates the FILES PRESENT can never detect a file that is ABSENT. Mine passed 16/16 while brand-guidelines.md — an always-required file — was missing from the master, because the loop compared each file it found to its MANIFEST row and a missing file is simply not iterated. Always check BOTH directions: every row has a file, and every file has a row. — Abid Siddiqui / 2026-09-01
- [2026-09-01] [CORRECTION] The worked examples in examples/ and templates/review-scorecard.md are NOW ALWAYS-REQUIRED READS, not optional reference. Proof: the same three-sentence nonprofit email was reviewed twice on 2026-09-01. The run that read examples/on-brand-approved.md returned APPROVED WITH CHANGES; the run that skipped it returned REJECTED. The submitted draft WAS that approved example with one clause deleted ("fewer manual reminders, more time with members"), so without reading the example you cannot see you are one clause from the approved bar — and you read a warning as a failure. Two further runs independently flagged the same gap unprompted. The specification gives you the output SHAPE; the example gives you the SEVERITY. Moved into the always-required table with the reason attached. — Abid Siddiqui / routing and consistency tests 2026-09-01
- [2026-09-01] [CORRECTION] Two bundled files give opposite instructions on the word "empower". banned-words.md bans "empower (overused)" with replacements help/enable/equip/support; the "Words We Use / Words We Avoid" table in brand-guidelines.md lists "Empower / Streamline" under USE. That table sits inside the section headed "Carried Forward From the Previous Version" — pre-May-2026 text reproduced so nothing was lost — and the ban was added later. RULE: the ban wins, say the sources conflict, escalate to Anna Klement. GENERALISED: anything under a "Carried Forward From the Previous Version" heading is preserved history, not current instruction, and loses to any rule stated outside such a section. Found by the skill itself during a live review, not by QA. — Abid Siddiqui / 2026-09-01
- [2026-09-01] [CORRECTION] SOURCES must now say when a read was PARTIAL ("— read in part: which sections"), must list the template and worked example used, and must state the skill version. Reason: a review cited master-icps.md flat in SOURCES having grepped roughly thirteen lines of it, which reads identically to having read the file end to end. A judgment resting on a fragment must not look like one resting on the whole file. The version matters because two copies of this skill can be installed under the same name and whichever wins is invisible to the reader. — Abid Siddiqui / 2026-09-01
- [2026-09-01] [WIN] Routing fix confirmed under adversarial phrasing with the competitor live. With daxko-brand-qa ENABLED, all four phrasings routed to daxko-brand-guardian — including "brand check this landing page" (the exact phrase that caused the 2026-08-24 hijack) and "QA this copy" (which daxko-brand-qa's own description explicitly claims). Every run also named which skill answered and which reference files it opened versus deliberately left closed. — Abid Siddiqui / 2026-09-01
- [2026-09-01] [PATTERN] Two installs of the same skill under the same name is a coin-flip the reader cannot see. The personal-skills copy wins over the plugin copy by default. They are byte-identical today; the moment the plugin is bumped and the symlinked master lags, a silently stale review is served with nothing in its output to reveal it. Also: in Claude Code the plugin is loaded @inline from disk, not from a registered marketplace, so Claude Code reach VIA THE MARKETPLACE is unproven and must not be inferred from a local test. — Abid Siddiqui / 2026-09-01
- [2026-09-02] [CORRECTION] Söhne versus Barlow is settled: **Barlow**, with Arial as web-safe fallback only, per Clint Malson citing the Daxko Brand Standards. Söhne is prohibited everywhere — including the product-lockup text exception that logo-guidelines.md Don't 8 used to permit, which is now closed. Fixed AT SOURCE in visual-brand/slide-layouts.md, layout-and-spacing.md, logo-guidelines.md and patterns-and-imagery.md, then re-bundled and shipped as v1.6.0 — not patched in the skill body, which is what D14's own rule demands so the other 73 agents inherit the correction. The skill's conflict table no longer says "escalate to Clint Malson"; a Söhne specification is now a violation to flag. Closes decision D14. — Abid Siddiqui / Clint Malson / 2026-09-02
