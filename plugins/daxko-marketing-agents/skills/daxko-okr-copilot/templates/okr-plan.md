# The OKR plan output format

Copy this shape exactly. **Same order, every time, without exception.** A plan's most dangerous failure is
a commitment nobody made reading as already agreed — so the shape is built to put a draft label first, the
inputs and assumptions second, and a visible placeholder wherever a human decision is still open.

This file gives you the **shape**. The worked examples in `examples/` give you the **standard**. Read the
template and both examples, every time.

---

## Which shape — decide before you write a word

| The reply is … | Shape | Offers in it |
|---|---|---|
| A **PLAN**, **RE-PLAN** or **CHECK** | **The spine** (below), with the body for the act | Exactly one — the closing line |
| A **P1 pause** — a gating input is still open after inference | **The P1 pause shape** | None |
| A **P2 pause** — a plan was asked for alongside a status or gap, or with results data to read | **The P2 pause shape** | Exactly one — the Agent 18 — Marketing Performance handover |
| The **no-objectives stop** — the period has no bundled objectives and none were pasted | **The no-objectives stop shape** | None |
| A **boundary decline** — the ask is out of scope, and no plan is in this reply | **The boundary decline shape** — no spine | At most one |
| A **STOP** — a required file is unusable | **The STOP shape** — no spine | None |
| A **partial plan** — a conditional file whose trigger fired is unusable | **The spine**, opened with the partial-plan line | Exactly one — the closing line |

---

## The spine — every plan, every size, this order

```
**DRAFT FOR DISCUSSION — nothing in this plan is agreed until its owners accept it.**

[Only when it applies, directly under the label:]
[The numbers you pasted were not read; nothing in this plan rests on them.]
[Partial plan — `references/[file].md` could not be read, so [what is affected].]
[Bundle-integrity note — `[file]` was absent and was read from another install of this same skill at this
 same version; its SHA-256 matched the MANIFEST.]

## Inputs and assumptions

- **Act:** [PLAN | RE-PLAN | CHECK]
- **Given:** [what the person gave, by name — the request, a pasted plan, pasted goals, Agent 18 — Marketing
  Performance's reading and its measurement date, any figure or constraint they stated]
- **Not given:** [what the plan would want and did not get, by name — a quarter's figure, an owner, a budget
  limit, a current count]
- **Inferred (not asked):** [each inference, one line each, marked "(inferred)" — the Key Results, the
  period, the scope]
- **Key Results planned against:** [each quoted word for word from the current tables of
  `references/okrs-and-priorities.md`, with its objective's name — never a "KR1"-style ID]
- **Period:** [the quarter or window, with its dates]
- **Status:** [Agent 18 — Marketing Performance's word, quoted exactly, with its source and measurement
  date — and for `cannot say`, the reason "no status rule has been set — owner: Abid Siddiqui"]
  | [your premise, quoted as yours: "You've told me … is behind"]
  | [Status: not assessed here — this plan reads no numbers]
- **Targets:** as bundled. `okrs-and-priorities.md` open questions 1, 3 and 7 ask whether they have been
  revised.

## The plan

[The body for the act — see "The bodies" below.]

## Key Results check

| Key Result (quoted) | What in this plan serves it | Quarter's figure |
|---|---|---|
| [quoted] | [item numbers and names] — or **"nothing in this plan serves it"** | [YOUR FIGURE, tagged] or `[QUARTERLY TARGET — not defined]` |

## Placeholders and decisions for a human

| # | Placeholder | Where it sits | The decision | Who decides | Where the gap lives |
|---|---|---|---|---|---|
| 1 | `[… — …]` | [item / section] | [what must be decided] | [a role — never a named person unless the person supplied the name] | [file and section, or "not in any bundled file"] |

[Every bracket in the plan has a row. Person-supplied premises and figures are listed here too, as
unverified. Never omit the section; where there are none, write:
"None — every commitment in this plan is sourced or supplied by you."]

## SOURCES

- references/corrections-snapshot.md | the writable corrections master — [N entries] | [none found — no
  corrections file present]
- references/okrs-and-priorities.md (as of [from MANIFEST]) — read in full
- references/performance-data-schema.md — as of [from MANIFEST] — read in part: Pipeline Attribution Model;
  Pipeline Coverage Targets; Core KPI Definitions; Market-Specific KPIs; Reporting Cadence; Performance
  Report Schema (rules in force) · Market-Specific Targets; Attribution Model (carried forward — read for
  their gaps only) · not used: Marketing KPIs; Data Sources; Pipeline Stages.
- references/[file].md (as of [from MANIFEST]) — read in part: [which sections] · or — read in full   ← each
  conditional file actually opened, and only those; "read in full" whenever the whole file was opened
- Not opened: [the conditional files whose trigger did not fire, in one line — so the reader can see the
  plan rests on none of them]
- references/MANIFEST.md — every "as of" date is read from here and never from a bundled file's own header
- Inputs: [Agent 18 — Marketing Performance's reading and its measurement date | person-supplied figures |
  pasted goals | a pasted plan | none]
- templates/okr-plan.md (output shape)
- examples/good-nonprofit-q4-plan.md (standard) · examples/bad-invented-commitments-plan.md (standard —
  annotated failure)
- SKILL VERSION: [read it off the SKILL VERSION line in SKILL.md]

## Next step

[One line — the first match in SKILL.md's next-step order. Name the agent by number and name, and offer
the sentence the person can reply with. Never a numbered menu, never two offers.]
```

---

## The bodies

### PLAN — the initiative table

```
| # | Initiative — what to do | Order | Owner (role) | Proposed timing | Key Result served (quoted) | Signal that would show it working | Depends on | Risks | Bet worth testing first | Built Daxko agent that can help |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | [what to do, in plain words] | [1st / after item N] | [a role, labelled proposed] or `[OWNER — to assign]` | [window within the quarter, labelled proposed] or `[DATE — depends on …]` | [the Key Result's name, quoted] | [a Key Result, or a KPI or funnel stage defined in Part A of performance-data-schema.md] or `[SIGNAL — no defined measure]` | [facts, people, products or spend it needs — with `[BUDGET — human decision]`, `[PRODUCT — confirm sellable in …]`, "Safe Harbor assessment before build — `daxko-agent-safe-harbor`" where they apply] | [what could stop it, sourced] | [one line, or "—"] | [live agents by number and name; others named "(not yet available)"; org skills named, never offered] |
```

Then, only where Step 6 of SKILL.md allows:

```
### Sizing

[Each sum on its own line, every input tagged TARGET / ASSUMPTION / GAP / YOUR FIGURE, the working shown:
 "$X (GAP, Agent 18 — Marketing Performance, measured [date]) ÷ $Y (ASSUMPTION, [file, section]) = Z".]

[What the sizing is not, in one line: not a quarter's target, not a forecast, not an impact —
 `[QUARTERLY TARGET — not defined]` · `[IMPACT — not estimated]`.]
```

**For "set team objectives":** in place of the initiative table —

```
| # | Team objective (in words) | Ladders to (quoted company or market Key Result) | Team-level signal | Team target |
|---|---|---|---|---|
| 1 | [objective] | [quoted] | [signal] | [YOUR FIGURE] or `[TEAM TARGET — not defined]` |
```

### RE-PLAN

The PLAN body, preceded by what it was built from:

```
**Built from:** [Agent 18 — Marketing Performance's reading, quoted — its status word exactly, its gap
arithmetic as it gave it, its measurement date] | [your premise, quoted: "…"]
```

### CHECK — two tables, never a judgement of success

```
**Items**

| # | Item (as you wrote it) | Key Result it serves (quoted) | Commitments resting on a fact not in the files |
|---|---|---|---|
| 1 | [item, owner names as given] | [quoted] — or **"serves no Key Result in the files"** | [an unsourced quarter's target · an unshipped product · an invented impact · a dependent date] — or "—" |

**Key Results**

| Key Result (quoted) | Items serving it |
|---|---|
| [quoted] | [item numbers] — or **"nothing in this plan serves it"** |
```

---

## The P1 pause shape — clarify once, then wait

```
Before I plan this — [N] things I have worked out, and [N] I need. Reply "yes" to use the defaults.

**Worked out:** [each inference, one line each]

1. **[The open gating input]:** [the question] *(default: [proposed default])*
2. **The quarter's figure for [each annual target]:** none set in the files *(default: none — marked
   `[QUARTERLY TARGET — not defined]`)*   ← rides along only because a pause is already happening
```

**No plan in this reply, and no offer.** The person's next message produces the plan, whatever it says.
Never a second round.

---

## The P2 pause shape — the reading first

```
I don't read numbers into a status or a gap — Agent 18 — Marketing Performance does, and I'll plan from
its reading.

Want me to hand this to Agent 18 — Marketing Performance to read where [the Key Result] stands from your
numbers? Once its reading is in this chat, I'll plan from it.
```

**The pasted numbers are not read — not summarised, not quoted, not used.** If the person declines or asks
for the plan anyway, the plan comes at once and opens with *"The numbers you pasted were not read; nothing
in this plan rests on them."*

---

## The no-objectives stop shape

```
The objectives for [period] are not in my files — the bundled OKRs are annual 2026 targets, running to
31 December 2026, and I never carry them forward as [year] targets.

Paste the company, market or team objectives for [period], and I'll plan against them as yours.
```

**No plan, no outline, no offer.** The last sentence is an instruction naming what to paste. Decline words
do not lift this stop.

---

## The boundary decline shape — no spine

```
[One or two lines: what was asked, and that it is not this agent's job — plainly, without apology.]

[The owner, by number and name, or the skill name — and its state: live / not yet available / a dead end.
 One line per ask when the message carried several.]

[At most one offer: the handover to a live Daxko agent; or, when there is no live owner and the request
 really contains planning, your own planning work; or nothing.]
```

**No draft label, no placeholders list, no SOURCES block.** A boundary decline is not a plan.

---

## The STOP shape — a required file is unusable

```
I can't make this plan. These required files could not be used:

- `[file]` — [missing | empty | truncated | holds no usable content | a Part A heading is missing]
- [every unusable file — never just the first]

The plan can't be made without them, and I won't plan from memory. [If a same-version install with a
matching checksum exists, say so; otherwise: "No same-version install holds the file."] Please tell Abid
Siddiqui so the bundle can be repaired.
```

**No plan, no outline, no partial plan, no offer.**

---

## Rules for filling it in

**The draft label is always first.** It is the cheapest defence against a proposal being read as a decision.

**Every commitment nobody has made is a bracket IN THE PLAN, and a row in the placeholders list.** A
quarter's target, an impact, a named owner, a budget, a product's availability, an agent's availability, a
dependent date, a status. Never a plausible number; never a vague hedge standing in for one.

**Owners are roles.** A person's name appears only when the person supplied it, and then it is listed as
person-supplied.

**Key Results are quoted word for word from the current tables**, with their objective's name. Never by an
ID.

**Every figure carries its kind** — TARGET, ASSUMPTION, GAP, YOUR FIGURE, ACTUAL — and an ACTUAL never
enters a sum.

**Read a file only in part, and say which part.** `performance-data-schema.md` is always declared in the
exact read-in-part form above. Any other file opened whole is declared "read in full" — declare what was
opened, not what was used. *(Corrected 2026-10-05, test run 3, Case 23.)*

**The "as of" date comes from `references/MANIFEST.md`, never from a file's own header.**

**One offer in the whole reply.** Every other owner is named, with its state — live, not yet available, or
a dead end — and not offered.
