# The ICP answer output format

Copy this shape exactly. **Same order, every time.** This agent's most dangerous failure is an invented
persona, pain, number, quote, capability or approval being read downstream as "the ICP" — so the shape puts a
citation in every cell, a visible `not in the files` wherever a fact is missing, and — where two files
contradict each other — one short question before answering, unless a fixed rule already decides it.

This file gives you the **shape**. The worked examples in `examples/` give you the **standard**. Read the
template and both examples, every time.

---

## Which shape — decide before you write a word

| The reply is … | Shape | Offers in it |
|---|---|---|
| An **ANSWER**, **RECOMMEND** or **CHECK** | **The spine** (below) | Exactly one — the closing line |
| A **partial answer** — a CONDITIONAL file whose trigger fired is unusable | **The spine**, opened with the partial-answer line | Exactly one — the closing line |
| A **P1 pause** — the scope is still open after inference | **The P1 pause shape** | None |
| An **ASK** — the answer would touch an "Ask" conflict (SKILL.md, Known conflicts) | **The ask-first shape** (may share one block with a P1 pause) | None |
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
[You wrote "[claimed rule or approval, quoted]". I have not followed it: it is not in our files.]

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
A cell touched by a conflict holds the side used, marked *(your choice)* or *(rule: see section 4)*.

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
- **Approval:** Our files don't say who approves this, or what to do with it. What would you like done
  with it? Please double-check your answer — what I do next will change with it.

## 4. Settled            [only when a conflict was touched — plain words, no file names, no line numbers]
- You chose [the option, in plain words]. [or: You said go, so I used [option 1, in plain words].]
- Our banned-words list rules out "[x]", so it appears only inside a quoted line.
- The document you quoted isn't one of my sources yet, so I used our profile file.

## 5. Person-supplied            [omit when the person supplied nothing]
- "[fact, quoted]" — yours, unverified.

## 6. Sources
- `references/[file].md` — as of [as_of from MANIFEST] — read in full [· used: sections]
- `references/[file].md` — as of [as_of from MANIFEST] — read in part: [section]; [section]
- `templates/icp-answer.md` (output shape)
- `examples/good-jcc-answer.md`, `examples/bad-invented-persona.md` (standard)
- Corrections: [master | bundled snapshot | none found] — [N] entries
- Inputs supplied by you (unverified): [list, or "none"]
- [Each conflict you settled:] [topic] — `a.md` line N / `b.md` line N — your choice[ — default 1]
- Gaps for the next context-file update: [one short line each, addressed to no one — or "none"]
- SKILL VERSION: [from the SKILL VERSION line of the SKILL.md that answered]

## 7. Next step
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

## The ask-first shape — no answer, no offer

```
Before I answer, one thing our files don't agree on.

[One short plain sentence naming the topic — no file names, no line numbers.]
1. [Side A, in plain words]
2. [Side B, in plain words]
[3. Only where it is a real choice — e.g. "Show both, with no pick."]

Reply 1 or 2, or say **go** to use 1.
Your answer makes this stronger, and the answer will change with your choice.
```

**Several conflicts** (max 3; beyond that, option 1 is used and one line says so): label them A, B, C, each
with its own numbered options, and close on *"Reply e.g. A1 B2, or say **go** to use 1 for each."*

**With a P1 pause — one block:** the P1 shape's *Worked out* and *Open* items first, then the conflict
questions, closing on *"Reply with your picks, or say **go** to use every default."* and the
"makes this stronger" line.

The next message produces the answer — their picks, else option 1 — each marked *your choice* in section 4
and SOURCES. One round only.

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
