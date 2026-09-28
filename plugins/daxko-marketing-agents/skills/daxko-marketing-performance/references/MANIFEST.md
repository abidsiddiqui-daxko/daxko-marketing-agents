# MANIFEST — bundled knowledge for Agent 18 — Marketing Performance

> ⚠️ **THIS FILE IS GENERATED. NEVER HAND-EDIT IT.**
> The check-up compares each recorded `source_checksum` against the current checksum of the source
> file to decide whether this bundled copy has gone stale. Edit a row by hand and the drift becomes
> invisible.

**Generated:** 2026-09-27 · **Agent:** Agent 18 — Marketing Performance · **Skill:** `daxko-marketing-performance` · **Skill version:** 1.7.6

> ⚠️ **On that version number.** 1.7.6 is the version of `plugin-daxko-agents` **as it stands on
> 2026-09-27**, read from `plugins/daxko-marketing-agents/.claude-plugin/plugin.json`. This build
> was built at 1.7.5 and SHIPPED in v1.7.6 on 2026-09-28; plugin.json, both skill bodies and every MANIFEST version line moved in that one commit (N25). The release that ships this skill must move `plugin.json`,
> the `SKILL VERSION:` line in `SKILL.md` **and this line** in the same commit (non-negotiable 25).

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
| `nonprofit-playbook.md` | `verticals/nonprofit-playbook.md` | `38cbf7152ec18875cd3f2c388b545699f32614f144de17b02b06d6d5c91cf279` | verbatim | 2026-09-27 | **2026-08-17** | 31 KB |
| `club-playbook.md` | `verticals/club-playbook.md` | `31dbb5897a42ee0a3e1f3fb8b7d9bc9a3d0b4060bd051af2dae00c4dae31c475` | verbatim | 2026-09-27 | 2026-08-05 | 17 KB |
| `boutique-playbook.md` | `verticals/boutique-playbook.md` | `eaa5b4182ce8a4f6f6cf39684ef5bca4b79d918cc9c8118916040ab5d9391c1b` | verbatim | 2026-09-27 | 2026-08-10 | 29 KB |
| `master-icps.md` | `knowledge-base/master-icps.md` | `06f2906660aee9d6144d8bd37d7c9f7db8a079e32e2653b748291a165ec3f27a` | verbatim | 2026-09-27 | 2026-08-05 | 19 KB |
| `product-knowledge.md` | `knowledge-base/product-knowledge.md` | `4d3d9d6ff9c166e04e40d468d4a56be5360b3a3196476ce39b10c7a53444b1a6` | verbatim | 2026-09-27 | **2026-09-18** | 23 KB |
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

## Three `as_of` dates that are NOT the date in the source file's own header

Shown in bold in the table above, plus one that needed checking rather than trusting.

| File | Header says | `as_of` recorded | Evidence |
|---|---|---|---|
| `nonprofit-playbook.md` | `LAST UPDATED: 2026-08-10` | **2026-08-17** | The content was corrected on 2026-08-17 — the AI-differentiation bullet was narrowed to the two capabilities in production today. File mtime agrees (2026-08-17). The header was never updated. Recorded as an inherited source condition in this agent's `SPEC.md` §8.3, and already an outstanding owner action against Agent 9 — Brand Guardian and Agent 13 — Content Production |
| `product-knowledge.md` | `LAST UPDATED: 2026-08-11` | **2026-09-18** | Its AI-capability section was restructured **by delivery status** on 2026-09-18, ruled by Abid Siddiqui, after four of six Daxko Engage Pro AI capabilities had been listed as delivered when `nonprofit-playbook.md` places two at Q3 2026 and two at Early 2027. Header still shows August |
| `okrs-and-priorities.md` | `LAST UPDATED: 2026-08-11` | 2026-08-11 | Header, mtime and checksum all agree. **The header is right about the file and still tells you nothing about the numbers** — see the section above |

### Three files whose mtime moved without their content moving — checked, not assumed

`product-knowledge.md` (mtime 2026-09-22), `club-playbook.md` (2026-09-22) and
`boutique-playbook.md` (2026-09-22) all carry a **later mtime than their `as_of`**. That looks like
drift and is not.

Each of their SHA-256 values above is **byte-identical** to the row Agent 13 — Content Production
bundled on 2026-09-17 and recorded in `agent-builds/agent-13-content-production/skill/daxko-content-production/references/MANIFEST.md`.
Identical bytes cannot be a content change, so the later mtime is a re-save, a copy or a touch.
`as_of` therefore stays at the date the **content** last changed, which is what a SOURCES block is
reporting when it quotes one.

⚠️ **This is why `as_of` is not simply `stat`-ed.** An mtime is a filesystem event; `as_of` is a claim
about content. Taking the first for the second would have aged three files by up to six weeks in
every SOURCES block this skill ever writes — invisibly, and in the safe-looking direction.

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
