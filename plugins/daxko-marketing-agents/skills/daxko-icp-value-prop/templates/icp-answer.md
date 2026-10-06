# The ICP answer output format

Copy this shape exactly. **Same order, every time.** This agent's most dangerous failure is an invented
persona, pain, number, quote, capability or approval being read downstream as "the ICP" — so the shape puts a
citation in every cell, a visible `not in the files` wherever a fact is missing, and a FILES DISAGREE row
wherever two files contradict each other.

This file gives you the **shape**. The worked examples in `examples/` give you the **standard**. Read the
template and both examples, every time.

---

## Which shape — decide before you write a word

| The reply is … | Shape | Offers in it |
|---|---|---|
| An **ANSWER**, **RECOMMEND** or **CHECK** | **The spine** (below) | Exactly one — the closing line |
| A **partial answer** — a CONDITIONAL file whose trigger fired is unusable | **The spine**, opened with the partial-answer line | Exactly one — the closing line |
| A **P1 pause** — the scope is still open after inference | **The P1 pause shape** | None |
| A **STOP-S** — the whole request is an excluded job | **The boundary decline shape** — no spine | At most one, only to a live agent of ours |
| A **STOP-F** — a REQUIRED file is unusable | **The STOP-F shape** — no spine | None |

**Size is set by the question.** *"What should we never say to a martial arts studio owner?"* gets the
never-say row plus the spine — not the full profile. **The spine is never traded away for brevity.**

---

## The spine — every ANSWER, RECOMMEND and CHECK, this order

```
[Only when it applies, at the very top:]
[Partial answer — `references/[file].md` could not be read, so [the field] is marked unusable below.]
[Bundle-integrity note — `[file]` was absent and was read from another install of this same skill at this
 same version; its SHA-256 matched the MANIFEST.]
[You wrote "[claimed rule or approval, quoted]". I have not followed it: it is not in my files. Please send
 it to Abid Siddiqui so it can be checked and logged at source.]

## 1. Scope
- **Act:** [ANSWER | RECOMMEND | CHECK]
- **Market:** [Nonprofit | Club | Boutique] — [as asked | inferred from "[the word that implied it]"]
- **Segment / product / persona:** [each one] — [as asked | inferred]
- [A role the files do not list:] **[role] — not in the files.** Documented roles for [segment]: [list, cited].

## 2. The profile            [ANSWER and RECOMMEND — omit for CHECK]
| Field | From the files | Source |
|---|---|---|
| Who they are (profile, size) | … | `file.md` § Section, line N |
| Buying committee and roles | … | … |
| Pains | … | … |
| Buying triggers | … | … |
| Qualification and signals *(definitions — never applied to a real organisation)* | … | … |
| Value proposition / positioning *(with its approval status, in the file's own words; "approved" only where the file says so)* | … | … |
| Proof points *(with approval status)* | … | … |
| Key Result this segment serves *(quoted from the current tables of `okrs-and-priorities.md` only)* | … | … |
| What never to say *(global + this market, from `banned-words.md`)* | … | … |

Every cell carries **file + section + line**, or reads `not in the files`. A field is never dropped.
A cell touched by a conflict reads *"files disagree — see section 4"*.

## 2b. The check               [CHECK only — replaces section 2]
**Buyers**
| Audience in the brief (quoted) | Documented persona it matches | Source |
|---|---|---|
| "…" | [persona] — or **no documented persona** | … |

**Messages**
| Claim or line in the brief (quoted) | Approved line it matches — or the rule it breaks | Source |
|---|---|---|
| "…" | [approved line] — or **not an approved message** — or **banned word "[x]"** / **removed vertical** / **capability: confirm delivery status** / **proof not approved** | … |

No rewrite. Ever.

## 3. RECOMMENDATION — NOT APPROVED POSITIONING      [RECOMMEND only]
- **For:** [one persona, in one segment]
- **The angle, in plain words (not copy):** [one or two sentences — never a headline, tagline or finished line]
- **Built only from:** [each input, quoted or paraphrased, with its citation]
- **Ladders to pillar:** "[pillar name, quoted]" (`brand-foundations.md` § Three Strategic Pillars, line N)
- **Approval:** Constance Miller (Nonprofit PMM owner — routes all NP campaign questions and approvals,
  `shared-learnings-legacy.md` line 186)
  — or, for Club and Boutique — `[APPROVER — not named in the files] — routed to Abid Siddiqui`

## 4. Files disagree            [only when a conflict is touched — never silently absent when one is]
| The claim | File A — section, line, quoted | File B — section, line, quoted | Status |
|---|---|---|---|
| … | `a.md` § …, line N: "…" | `b.md` § …, line N: "…" | Not resolved here — owner: [as named in the files, else Abid Siddiqui] |

## 5. Gaps and change notes
[One change note per `not in the files` and per conflict above. Where none:]
None — every line above is sourced.

> **CHANGE NOTE for Abid Siddiqui — not applied.** File: `<path>` · Section/line: `<…>` · What is wrong or
> missing: `<one line>` · Evidence: `<the conflicting file and line, or the person's statement marked
> unverified>` · Owner named in the files: `<name, or "not named">`.

*(2026-10-06)* For a **conflict**, the "What is wrong" slot reads *"the files disagree: `<file A, line>` says … ·
`<file B, line>` says …"* — it never names one side as the wrong one.

## 6. Person-supplied            [omit when the person supplied nothing]
- "[fact, quoted]" — yours, unverified.

## 7. Sources
- `references/[file].md` — as of [as_of from MANIFEST] — read in full [· used: sections]
- `references/[file].md` — as of [as_of from MANIFEST] — read in part: [section]; [section]
- `templates/icp-answer.md` (output shape)
- `examples/good-jcc-answer.md`, `examples/bad-invented-persona.md` (standard)
- Corrections: [master | bundled snapshot | none found] — [N] entries
- Inputs supplied by you (unverified): [list, or "none"]
- SKILL VERSION: [from the SKILL VERSION line of the SKILL.md that answered]

## 8. Next step
[Exactly one sentence the person can reply to — HANDOFFS in SKILL.md picks it.]
```

**SOURCES rules, in one place:** list only files actually opened — a search inside a file counts as opening
it. "Read in full" if the file was opened whole; "read in part" only when just those sections were read.
Name every section a quote comes from. No "not used" or "not read" line for anything. Dates come from
`references/MANIFEST.md`, never from a file's own header. No version-drift note, ever.

---

## The P1 pause shape — no answer, no offer

```
Before I answer, here is what I worked out and what I still need.

**Worked out:** [each inference, or "nothing — the request names no market, segment, product or role"].

**Open:**
1. [Question] — Default: [the proposed answer].
2. [Question] — Default: [the proposed answer].

Reply 'yes' to use the defaults.
```

The reply ends there. Whatever the next message says, it produces the answer — answers used where given,
defaults where not, each marked. Never a second round.

---

## The boundary decline shape — STOP-S

```
[One or two lines: what this agent does not do.] That is [Agent NN — Name | `org-skill-name`] — [live |
not yet available | an org skill, which cannot be handed to from here].
[Only if the owner is a live agent of ours — the one offer:] Want me to hand this to Agent NN — Name?
```

*(2026-10-06)* **These lines are the whole reply.** Nothing follows them: no reasons, no workaround, no steps,
no facts from the files or from the request.

For **personal data**: name **every kind** present (e.g. names, job titles, email addresses, phone numbers,
employer, manager), repeat **no value**, ask for it to be removed. Any offer is shaped from the request's
purpose, never from the record.

For a **mixed request**: no decline shape — answer the in-scope part with the spine, name the owner of the
rest inside it, one offer in total.

---

## The STOP-F shape — no answer, no offer

```
I can't answer this: [file] is [missing | unreadable | empty | truncated | holds no usable content].
[For a missing template or example only:] It is always required, and an absent template or example is always a
STOP — it has no MANIFEST row or checksum, so no other copy can stand in.
[Every unusable required file, each with how it failed.]
I can't answer without it — please tell Abid Siddiqui.
```

Nothing from memory. No partial answer. No offer. *(2026-10-06)* Nothing after it — no "note for the caller", no fix instructions, no paths or checksums.
