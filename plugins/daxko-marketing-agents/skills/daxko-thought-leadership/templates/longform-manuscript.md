# The long-form manuscript output format

Copy this shape exactly. **Same order, every time, without exception.** A whitepaper drafted off an
unapproved outline can waste a great deal of prose on the wrong structure — so the shape is built to **lock
the thesis and outline first, offer them, then draft.**

This file gives you the **shape**. The worked examples in `examples/` give you the **standard**. Read one of
each, every time.

---

## Step A — LOCK, then OFFER (the default two-step flow)

```
**Asset type:** [whitepaper / eBook manuscript / industry or research report / executive byline article]
**Market:** [nonprofit / club / boutique / market-neutral]   ·   **Audience:** [the buyer/role the piece is written for]
[For a byline article: **Byline:** whose voice this is ghostwritten in.]
[If anything was inferred rather than stated, say so here in one line each.]
[If no market was named: "Written market-neutral — no market was named, so no market's voice rules were
 applied and no playbook was opened."]

## Title + thesis + outline

**Working title:** [the title]

**Thesis:** [the single sentence the whole piece argues. One sentence. Everything in the piece serves it.]

**Outline**
1. [Section header] — [one line on what it covers]
2. [Section header] — [one line on what it covers]
   … [as many as the piece needs]

**The one action:** [what the reader should do at the end] → [where it goes]

> **Here is the thesis and outline. Want me to draft the full manuscript from this, or adjust the outline
> first?**
```

🔴 **The offer is made exactly once — then the reply ends and waits.** Only the person's own words skip this
gate (*"just write it"*, *"skip the outline"*, *"no outline"*, *"write the full thing now"*, or a plain
equivalent). Never decide for them that the request is detailed enough to skip it. When they do decline the
gate, go straight to Step B in the same reply, and mark every assumption you had to make (assumed thesis,
assumed market, assumed audience) so it can be corrected after the draft, not before it.

---

## Step B — DRAFT (on approval, or immediately if the user declined the gate)

```
## The outline, as drafted

[The section list restated exactly as delivered below, so the reader can see the structure at a glance.]

## The manuscript

### [Section 1 header]

[The prose, ready to paste. Daxko voice for the named market and byline. Every unsourced fact appears as a
 visible [PLACEHOLDER — what is needed] at the point in the sentence where the claim was wanted — never a
 plausible number, never a vague hedge in place of one.]

### [Section 2 header]

[…and so on, in outline order, to the end of the piece.]

## SOURCES

- references/[file].md (as of YYYY-MM-DD)
- references/[file].md (as of YYYY-MM-DD) — read in part: [which sections]
- references/MANIFEST.md — every "as of" date is read from here and never from a bundled file's own header
- templates/longform-manuscript.md (output shape)
- examples/[file].md (standard)
- Corrections: [N entries found in <which file>] | [none found — no corrections file present]
- SKILL VERSION: [read it off the SKILL VERSION line in SKILL.md]

## Placeholders and gaps

| # | Placeholder | What is needed | Who supplies it |
|---|---|---|---|
| 1 | `[PLACEHOLDER — needs a sourced figure]` | [what claim was wanted and why no bundled file supports it] | [role or team] |

[Every bracketed item in the prose above appears here. If there are none, write "None — every claim in this
 manuscript is sourced to a bundled file." Do not leave the section out — for a long-form authority asset
 this list is a safety feature, not an afterthought.]

## Mapped KR

**[The key result, quoted as it appears in references/okrs-and-priorities.md]**

[One or two lines on how this piece serves it. If it genuinely maps to no KR, say so — do not force a mapping.]

## Next step

[One line. Name the next agent by number and name and offer to hand over — a sentence the person can reply to.]
```

---

## Rules for filling it in

**Lock the thesis first, always.** One thesis, one outline, before a paragraph of prose. A long piece written
without a locked thesis wanders, and the wandering is expensive to unpick after the fact.

**Order is fixed.** Title + thesis + outline, then the offer, then — on approval or an explicit "just write
it" — the drafted prose, then SOURCES, then Placeholders and gaps, then the mapped KR, then the one-line next
step.

**Every factual claim names its file or becomes a placeholder.** A statistic, a customer, a quote, a price, a
date or a product capability that you cannot find in a bundled file is a `[PLACEHOLDER]` in the prose and a
row in Placeholders and gaps — never a plausible number, and never a vague hedge standing in for one.

**A `[PLACEHOLDER]` stays visibly bracketed in the prose.** Do not write around it, do not soften it into
something vague, and do not quietly drop the sentence that needed it. The gaps list is a note to the
commissioner; the bracket in the sentence is a warning to whoever pastes it into the finished document. Both
are required, and the bracket is the one that travels.

**Read a file only in part, and say which part.** Write `— read in part: [sections]` in SOURCES. A judgment
resting on a fragment must not look like one resting on the whole file.

**The "as of" date comes from `references/MANIFEST.md`, never from a file's own header.** Several bundled
files carry a header date that is wrong about their own content.

**Casing** (`references/brand-guidelines.md`): sentence case for headings, subheadings and body; Title Case
for CTA labels and product names. **Full product names on first use** — "Zen Planner", not "ZP".

**One art-direction note in words is allowed; a design is not.** "Cover: a studio owner reviewing a report at
the front desk" is in scope. No colour value, no font, no layout — those belong to Agent 29 — UX/UI Design.

---

## The partial-manuscript shape — when one conditional file is unusable

If a **conditional** file whose trigger has fired cannot be read — the piece makes a competitive claim and
`references/competitive-intel.md` is unreadable, say — you do **not** refuse. You lose part of one thing, not
the manuscript:

- Write every section that does not depend on it.
- For the part that does, put a `[PLACEHOLDER]` in the prose and a row in Placeholders and gaps naming the
  file that could not be read.
- Say plainly at the top: **"Partial manuscript — `[filename]` could not be read, so [what is affected]."**
- Never guess the part you could not check, and never quietly leave the claim out as though it was never
  wanted.

**A REQUIRED file is different: if one is unusable, you produce no manuscript at all** — not a draft, not an
outline, not one section. `SKILL.md` Step 4 has the exact rule and the one narrow substitution that is
permitted.
