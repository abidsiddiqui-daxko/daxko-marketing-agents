# MANIFEST — bundled knowledge for Agent 18 — Marketing Performance

> ⚠️ **THIS FILE IS GENERATED. NEVER HAND-EDIT IT.**
> The check-up compares each recorded `source_checksum` against the current checksum of the source
> file to decide whether this bundled copy has gone stale. Edit a row by hand and the drift becomes
> invisible.

**Generated:** 2026-09-27 · **Agent:** Agent 18 — Marketing Performance · **Skill:** `daxko-marketing-performance` · **Skill version:** 1.7.9

> ⚠️ **On that version number.** 1.7.9 is the version of `plugin-daxko-agents` **as it stands on
> 2026-10-05** (v1.7.8 changed only the plugin description; v1.7.9 only Agent 11's skill description — this skill's content is unchanged since v1.7.7), read from `plugins/daxko-marketing-agents/.claude-plugin/plugin.json`. This skill
> was built at 1.7.5, first SHIPPED in v1.7.6 on 2026-09-28, and re-shipped in v1.7.7 on 2026-10-05 with
> the shared-file corrections re-bundled; plugin.json, every skill body and every MANIFEST version line
> moved in that one commit (N25). Every release that ships this skill must move `plugin.json`, the
> `SKILL VERSION:` line in `SKILL.md` **and this line** in the same commit (non-negotiable 25).

**What the columns mean**

| Column | Meaning |
|---|---|
| `bundled_file` | The copy inside this skill's `references/` folder |
| `source_file` | Where it came from in the Agent HQ source of truth |
| `source_checksum` | `shasum -a 256` of the **SOURCE** file at bundling time. The check-up re-runs this and compares |
| `fidelity` | `verbatim` = byte-for-byte copy · `excerpt` = part of the source · `converted` = reformatted |
| `bundled_on` | When this copy was taken |
| `as_of` | The source document's own last-changed date — this is what the SOURCES block reports |

---

| bundled_file | source_file | source_checksum | fidelity | bundled_on | as_of | size |
|---|---|---|---|---|---|---|
| `performance-data-schema.md` | `knowledge-base/performance-data-schema.md` | `6de5a39ed2394de335c310e5ffc018977a0fd3fb89883cbb35a3b471479891e7` | verbatim | 2026-09-27 | 2026-08-11 | 11 KB |
| `okrs-and-priorities.md` | `knowledge-base/okrs-and-priorities.md` | `52d169ac5aa287cda7315cb75937a362680ce18be1014d7c5125e4bdf32ef5cf` | verbatim | 2026-09-27 | 2026-08-11 | 12 KB |
| `nonprofit-learnings.md` | `verticals/nonprofit-learnings.md` | `71deb914759481cf68ffdfb47c1eb8d34efdfbf936c296eff0a9e2b10ac73357` | verbatim | 2026-09-27 | 2026-08-05 | 3 KB |
| `club-learnings.md` | `verticals/club-learnings.md` | `dd3b74574fc03522ce0ef0c48c06894e17de4f29af72f9db6fc01f33865cc071` | verbatim | 2026-09-27 | 2026-08-05 | 7 KB |
| `boutique-learnings.md` | `verticals/boutique-learnings.md` | `9cab2245798aa84783f264c558a04f07c1eeab4da3884650ecb851411db302ad` | verbatim | 2026-09-27 | 2026-08-05 | 7 KB |
| `nonprofit-playbook.md` | `verticals/nonprofit-playbook.md` | `735e94322cbe7d2a445e65e8836dbd2a5d094e4f0a318d1dcc52cb550bc09c66` | verbatim | 2026-10-05 | 2026-10-05 | 32 KB |
| `club-playbook.md` | `verticals/club-playbook.md` | `a8ff458cc99f070904447bc7a5c0efc042516820cfff84f9058c33cd03b2b37c` | verbatim | 2026-10-05 | 2026-10-05 | 18 KB |
| `boutique-playbook.md` | `verticals/boutique-playbook.md` | `740900c3f36648e2f315809cc452bbec60e9fce20c155b8199c8cbcc3c7e4893` | verbatim | 2026-10-05 | 2026-10-05 | 30 KB |
| `master-icps.md` | `knowledge-base/master-icps.md` | `6f6f0b560c67683b5bc672352e544939dbaf4b708ba1129a7e43f88af5dd7e7c` | verbatim | 2026-10-05 | 2026-10-05 | 19 KB |
| `product-knowledge.md` | `knowledge-base/product-knowledge.md` | `17e1fde5b9b71523e4847053e60f82793807b029f0b73cc4cb6426fe8f403332` | verbatim | 2026-10-05 | 2026-10-05 | 23 KB |
| `corrections-snapshot.md` | `learnings/agent-18-marketing-performance.md` | `3b90435e08c4bf8a357b18a1bde6948059d15177d360f7f7009352224ac1fa50` | converted | 2026-09-27 | 2026-09-27 | 5 KB |

**11 rows.** `MANIFEST.md` has no row for itself — it is the index, not bundled knowledge.

---

## The both-directions verification, and exactly what it enumerated

Non-negotiable 18: *"Every MANIFEST row must have a file, **and** every file in `references/` must
have a MANIFEST row… any 'everything matches' claim must say what it enumerated."*

| Direction | What was enumerated | Count | Result |
|---|---|---|---|
| **Row → file** | Every `bundled_file` value in the table above, checked for a file of that name in `references/` | **11 rows** | 11 of 11 present |
| **File → row** | `references/*.md` **minus `MANIFEST.md`**, checked for a row | **11 files** | 11 of 11 have a row |

The two counts are stated separately on purpose. **They are different questions**, and a single
"everything matches" would hide which one was actually asked — which is the defect that produced
non-negotiable 18: a loop over the files it found reported 16 of 16 correct while an always-required
file was missing from the master entirely.

`templates/` and `examples/` are **not** in this table and must not be added to it. They are
always-required reads (non-negotiable 19) but they are this skill's own artefacts, not bundled copies
of an Agent HQ source, so they have no `source_file` and no `source_checksum` to drift against.

---

## 🔴 The `as_of` date is NOT the date the numbers were measured

This warning belongs at the top of this file rather than buried in it, because for **this** agent it
is not a footnote — it is Law 2, and this skill's single most consequential rule.

`as_of` is **when the file was last changed.** It is not when any figure inside it was measured.

The live example is in this very table. `okrs-and-priorities.md` carries `as_of 2026-08-11`, and the
only attainment table it contains is headed *"**Current** attainment (April 2026 actuals)"*. So:

| | Value | What it is |
|---|---|---|
| The file's `as_of` | 2026-08-11 | When the document was last written |
| The measurement date of `$10,240,700` | **April 2026** | When the pipeline figure was actually taken |
| The word *"Current"* above it | — | 🔴 **An authoring artefact. Not a date, and not evidence of one.** |

Quoting `2026-08-11` for that figure would overstate its freshness by more than three months, and
quoting the word *"Current"* would overstate it by five. **Report the measurement date, and say how
old it is.** The MANIFEST date belongs in SOURCES, against the *file*; it never travels next to a
number.

---

## `as_of` dates that are NOT the date in the source file's own header — none, as of 2026-10-05

*Rewritten 2026-10-05, recomputed from the files.* This section listed three. `nonprofit-playbook.md` and
`product-knowledge.md` were corrected again at source on 2026-10-05 with their headers updated, so header and
`as_of` now agree (2026-10-05). `okrs-and-priorities.md` always agreed — header, content and checksum, 2026-08-11
— and **the header is still right about the file and still tells you nothing about the numbers** (see the
section above).

### Correction — the former sub-section "Three files whose mtime moved without their content moving"

That sub-section concluded that `product-knowledge.md`, `club-playbook.md` and `boutique-playbook.md` carried a
later mtime than their `as_of` because of a re-save, not a content change, on the grounds that their checksums
matched rows Agent 13 — Content Production "bundled on 2026-09-17". **That conclusion was wrong.**
`club-playbook.md` and `boutique-playbook.md` each carry a content correction dated 2026-09-22, and the same
2026-09-22 batch changed `product-knowledge.md` (25M+ → 20M+). The checksums matched because Agent 13 — Content
Production's MANIFEST had been re-bundled after 2026-09-22 while keeping its old dates — the stale-date defect
logged as F-2 by Agent 11 — Thought Leadership & Long-Form's test suite. All three rows were corrected on
2026-10-05.

⚠️ **The lesson stands, and is sharper:** an mtime is not an `as_of` — and neither is a date copied from another
MANIFEST. Read the dated correction markers inside the file itself.

---

## Note on `corrections-snapshot.md`

It has a row like any other bundled file — that is deliberate, and it is the whole point. Its source
is the **writable corrections master**, which lives outside every skill because a shared skill is
read-only for everyone who receives it. When a correction is logged, the master's checksum changes
and stops matching the row above. **That mismatch is how the check-up notices that corrections have
been logged but never published** — which would otherwise mean every correction stayed on one laptop
while teammates kept getting the same answer.

It must be re-copied, and this row updated, **at every publish, before the change that publishes**
(non-negotiable 11).

### Verifying it — it is the one exception

Every other row is `verbatim`, so the bundled copy's own checksum equals the recorded
`source_checksum`, and one comparison proves both that the copy is faithful and that the source has
not moved on.

**This file is `converted`:** its header is replaced at bundling time so the shipped copy does not
claim to be the writable master, and the *"How to add a correction"* section is removed because
nobody receiving the skill can act on it — the defect Agent 9 — Brand Guardian shipped once. Its
bundled bytes therefore differ from the source's bytes **by design**, and the two checks must be done
separately:

| Check | How |
|---|---|
| **Has the source moved on since the last publish?** | `shasum -a 256` the writable master and compare to the `source_checksum` above. **A mismatch means corrections have been logged but never published** — refresh the snapshot and republish. This is the alarm the row exists for |
| **Is the bundled copy faithful?** | Compare the correction lines only, not the header: `grep -c '^- \[20'` on both files must give the same number, and a `diff` of those lines must be empty. **At this build both are 0** — the master was created on 2026-09-27 and holds no entries yet |

⚠️ **Do not "fix" a mismatch by writing the bundled copy's checksum into the row.** That silences the
alarm instead of answering it.

---

## What is deliberately NOT bundled

| Not bundled | Why |
|---|---|
| `knowledge-base/brand-guidelines.md`, `knowledge-base/banned-words.md`, `knowledge-base/brand-foundations.md` | Blank in the Performance column of the root `CLAUDE.md` context matrix. This agent writes analysis, not marketing copy. 🔴 **The consequence is stated rather than hidden: this agent's output is not brand-checked.** When an answer is destined for a client — which ruling 3 makes routine — the next step offered is **Agent 9 — Brand Guardian** |
| **Everything in `visual-brand/`** | Not opened by this agent at all (`SPEC.md` §8.1). It specifies no colour, no font and no layout. Those belong to **Agent 29 — UX/UI Design** |
| `knowledge-base/competitive-intel.md` | Blank in the Performance column. A competitor's numbers are not Daxko's performance, and reading them invites the comparison this agent is not scoped to make |
| `knowledge-base/product-marketing-context.md` (67 KB) | Overlaps `product-knowledge.md`, which is bundled. Two competing product documents inside one analyst is how two different answers get given to one question |
| `knowledge-base/shared-knowledge-base-index.md`, `shared-learnings-legacy.md` | An index of the old system, and legacy learnings superseded by the per-market learnings files bundled above |
| `verticals/club-competitive.md`, `market-strategists-overview.md`, the YMCA / JCC / BGC and martial-arts / functional-fitness sub-playbooks | Sub-segment and competitor depth is content context. This agent needs market context only far enough to make a finding intelligible — §8.1 of `SPEC.md` makes the three market playbooks on-demand for exactly that reason, and goes no deeper |
| Anything in `drop-your-updated-files-here/` | ⛔ **Forbidden source.** It is older than the live folders |
| Any live org skill's bundled `references/` | ⛔ **Forbidden source.** `daxko-brand-qa` ships a months-old fork of `typography-system.md` still naming Söhne, against decision D14 — the font is **Barlow**. The same hazard applies to any analytics or finance skill's bundled figures, which is the form it would take here |
| Anything in `reference-material/` | Background reading from the previous system. Never bundled into a skill |

Adding any of these later means adding a row above at the same time, in the same commit.

## Change log

- **2026-10-05** — re-bundled from source after the shared-file corrections found by Agent 11 — Thought Leadership & Long-Form's test suite: every row above whose file was corrected today now carries the new checksum, bundled_on 2026-10-05 and as_of 2026-10-05. Rows whose file carries a 2026-09-22 correction but still recorded an older as_of were corrected to 2026-09-22 (finding F-2). Checksums of all other rows unchanged.

- **2026-10-05** — re-bundled from source after the shared-file corrections found by Agent 11 — Thought Leadership & Long-Form's test suite: every row above whose file was corrected today now carries the new checksum, bundled_on 2026-10-05 and as_of 2026-10-05. Rows whose file carries a 2026-09-22 correction but still recorded an older as_of were corrected to 2026-09-22 (finding F-2). Checksums of all other rows unchanged.
