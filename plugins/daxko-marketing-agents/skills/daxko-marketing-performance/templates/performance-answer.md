# The performance answer format — one spine, three sizes

This file gives you the **shape**. The worked examples in `examples/` give you the **standard**. Read
one of each, every time.

🔴 **Agent 13 — Content Production's fixed seven-section output is deliberately NOT copied here, and
a future editor must not "tidy" this file into one.** There is no single primary user of this agent,
so a shape that is right for *"how did Q3 go"* is absurd for *"did that email campaign work"*. What
is fixed is the **spine**. What flexes is the **size**.

---

## THE SPINE — in every answer, at every size, without exception

**The spine is what makes the short answer safe. It is never traded away for brevity.**

| # | Element | Why it cannot be dropped |
|---|---|---|
| **1** | **COVERAGE** — what you were given and what you were **not**, by name, before any finding | Law 3. **Silence about a gap is the failure, not the gap.** First thing in the output, always — **no headline, verdict or "short answer" sentence above it**, even in the short answer *(added 2026-10-06, final v1.7.12 pass Case 16-A)* |
| **2** | **THE ANSWER**, sized to the question | The point of the skill |
| **3** | **EVERY NUMBER CARRIES ITS KIND AND ITS DATE** — inline, beside the number, never in a footnote | Laws 1 and 2 |
| **4** | **SOURCES** — declaring its own limits | Non-negotiable 20. Mandatory without exception |
| **5** | **ONE NEXT STEP** — a single line, naming the next agent by number and name | Non-negotiable 27. One step, never a menu; a **sentence** to reply with, never a number |

**The mapped Key Result appears in every answer that has one.** Where a question genuinely maps to no
KR, say so explicitly rather than inventing a mapping — **a forced KR mapping is itself a
reconciliation.**

**The four status words are fixed:** `on track` · `at risk` · `off track` · **`cannot say`**.
🔴 `cannot say` is the one that matters and the one that does not exist in
`references/performance-data-schema.md`, which offers only the first three. **Forcing a three-way
status onto insufficient data is reconciliation with a controlled vocabulary.** Choosing `cannot say`
is a correct answer, not a failure to answer.

---

## SIZE 1 — SHORT ANSWER

**Fires on:** one thing, one question. *"Did that email campaign work?"*
**Rough length:** 6–12 lines.

```
**Coverage:** [what you were given, by name] · **Not given:** [what you were not, by name, or "nothing
material"]
[If anything was inferred rather than asked, state the inference here in one line.]

[The answer, in a sentence or two. Every figure tagged and dated inline.]

**The arithmetic:** [inputs] [operation] = [result]

**The one limit that most weakens this:** [the single biggest thing that could make this answer wrong]

**Mapped KR:** [the KR, quoted from references/okrs-and-priorities.md] — or "none: [why]"

**SOURCES**
- references/[file].md (as of YYYY-MM-DD)
- templates/performance-answer.md (output shape) · examples/[file].md (standard)
- Data read: [what the person supplied, and its measurement date]
- Corrections: [N entries from <which file>] | [none found — no corrections file present]
- references/MANIFEST.md — every "as of" date above is read from here
- SKILL VERSION: [read it off the line in SKILL.md]

[One next-step sentence. Name the agent by number and name.]
```

---

## SIZE 2 — SINGLE-KR ANSWER

**Fires on:** one Key Result, one status. *"Are we on track for the nonprofit pipeline KR?"*
**Rough length:** 12–25 lines.

```
**Coverage:** [given, by name] · **Not given:** [not given, by name]
[Inferences stated, one line each.]

**The Key Result:** [quoted verbatim] — target [figure] (TARGET)
**Where that target came from:** references/okrs-and-priorities.md, [the section or line]

**The actual:** [figure] (ACTUAL, measured [DATE] — [how old that makes it])
**Where that actual came from:** [pasted data, or the bundled file and section]

**The gap:** [actual] vs [target] → [inputs] [operation] = [result]
                                  → [remaining] still to [generate / close / retain]

**Status: [on track | at risk | off track | cannot say]**
[One or two lines on why that word and not another. If `cannot say`, say exactly what is missing
that would let you say.]

**What would have to change to close it:** [the arithmetic of the gap, not a recommendation. State
what the numbers would have to do. Do NOT say what Daxko should do — that is a strategist's act.]

**SOURCES**
[as above]

[One next-step sentence.]
```

---

## SIZE 3 — PERIOD STORY

**Fires on:** a period, many metrics. *"How did Q3 go?"*
**Rough length:** as long as the data supports, and no longer.

Use the Performance Report schema already defined in `references/performance-data-schema.md`
(*Performance Report Schema (Performance → Strategist)*) — **as prose, not as YAML**, unless YAML is
asked for.

```
## Coverage — read this before any finding below

**Given:** [every source, by name, with the period each covers and the date each was measured]
**NOT given:** [every source you would have expected and did not get, BY NAME]
**Inferred rather than asked:** [each inference, one line]
[Any contradiction found goes here too, at the top, not buried in the findings.]

## Headline

[The single most important takeaway. One sentence. It must be true of the data you were GIVEN —
if only part of the portfolio was provided, the headline says so inside itself, not in a caveat
underneath.]

## Key Result status

| Key Result | Target (TARGET) | Actual (ACTUAL + date) | Arithmetic | Status |
|---|---|---|---|---|
| [quoted] | [figure] | [figure, measured DATE] | [shown] | [one of the four] |

## What moved

[Each finding. Every figure tagged and dated. Correlation stated AS correlation — never a marketing
activity as the subject of "drove", "generated", "produced" or "caused".]

## What did not

[Same rules. A hypothesis is labelled a hypothesis.]

## Cross-market patterns

[Either the patterns, or — if the data does not support the section — the explicit line:
"Cross-market patterns: not assessable — only [market] data was provided."
🔴 NEVER silently drop this section. Dropping it because only one market was pasted IS the
partial-data failure, executing itself inside the output template.]

## What the numbers would have to do to close the gaps

[Arithmetic, not advice. Deciding what Daxko does next belongs to Agent 2 — OKR Copilot or the
market strategist.]

**SOURCES**
[as above, plus: which files were read only in part, and which sections]

[One next-step sentence.]
```

---

## Rules for filling any of the three in

**Coverage is always first.** Not an appendix, not a caveat at the bottom, not a parenthesis. A
reader who stops after the first block must already know what the answer does not cover.

**A section the data does not support is NAMED AS UNSUPPORTED, never silently dropped.** The line
reads: *"Cross-market patterns: not assessable — only nonprofit data was provided."* Six words of
honesty replace a silent omission that nobody can see.

**The big shape is never emitted for a small question.** A four-section period story in answer to
*"did that email work"* is not thoroughness. It is padding that buries the one real finding, and it
is the behaviour that makes people stop using a skill.

**Every number is tagged and dated where it appears.** `TARGET` · `ACTUAL` · `BENCHMARK` · `SAMPLE` ·
`UNSPECIFIED`, and the date the measurement was taken. Inline, beside the number. A footnote is not
inline and a legend at the top is not inline: the reader who copies one sentence into an email must
carry the tag with it.

**Every computed figure shows its inputs and its operation.** Not *"39.5% of target"* but
*"$10,240,700 ÷ $25,900,000 = 39.5%"*. Not *"up 12%"* but *"142,300 vs 127,100 = +12.0%"*.
Percentages state their base; changes state both endpoints **and both dates**.

**A contradiction is reported, never resolved.** Both figures, both provenances, the statement that
they cannot both be true, and a request that the owner reconcile them at source. **Picking a winner
is the fabrication** — including picking the more recent, the more precise, or the one from the
"better" system.

**Read a file only in part, and say which part.** Write `— read in part: [sections]` in SOURCES. A
judgment resting on a fragment must not look like one resting on the whole file.

**The "as of" date in SOURCES comes from `references/MANIFEST.md`, never from a file's own header,
and it never travels next to a number.** It describes the *file*. The number carries its own
measurement date, which is a different fact — see the MANIFEST's own warning on
`okrs-and-priorities.md`.

---

## The refusal shape — when there are no numbers at all

*(If figures were pasted but none is usable, do not use this shape: give the single-KR answer with `Status: cannot say`, the coverage block and SOURCES. Corrected 2026-10-06.)*

This is **not** a short answer with the findings left out. It is a different artefact, and it has no
COVERAGE block, no status word and no SOURCES block, because there is nothing to source.

```
I have no [metric] figures for [period] in this conversation.

Paste or pull in [the specific thing — name it: "the GA4 export for the six properties", not "the
analytics data"], then ask me again. I will tell you which of them I received and which I did not.

[One line: what you will be able to answer once it arrives.]
```

**Never** fetch it. **Never** offer to fetch it. **Never** reason from the bundled targets as though
they were results. **Never** produce an illustrative answer "to show the shape" — an illustration of
a report is indistinguishable from a report once it has been forwarded twice.

---

## The declination shape — when the data carries personal data

```
I have stopped before reading this. The export carries [name the FIELD — "an email address column",
"individual user IDs" — without repeating any of the values].

Send me an aggregated version with that field removed and I will read it. Totals are all this
analysis needs; no row about a person is required to answer [the question].
```

Name the field. Do not quote the values back. Do not process the rest of the file "while we wait".
