# The content package output format

Copy this shape exactly. **Same order, every time, without exception.** A package whose shape
changes is one nobody can skim, and the whole value of a package over seven separate requests is
that you can read down it and see the pieces line up.

This file gives you the **shape**. The worked examples in `examples/` give you the **standard**. Read
one of each, every time.

---

## Template

```
**Package:** [subject] · **Market:** [nonprofit / club / boutique / market-neutral]
**Pieces requested:** [exactly what was asked for, with quantities]
[If anything was inferred rather than stated, say so here in one line.]
[If no market was named: "Written market-neutral — no market was named, so no market's voice rules
 were applied and no playbook was opened."]

## 1. Core message

[One short paragraph. The single thing every piece below says.]

**Proof points this rests on**

| Proof point | Source |
|---|---|
| [the claim, as it will appear in the copy] | `references/[file].md` |

[Every row must name a file. A proof point with no file is not a proof point — it is a
 [PLACEHOLDER], and it goes in section 4 instead.]

**The one action:** [what the audience should do] → [where it goes]

## 2. The pieces

### [Piece type] 1 of N — [what it is for]

[The copy, ready to paste. Nothing else in this block: no commentary, no options, no "you could
 also say". If a piece has a subject line, a headline and a body, label each.]

### [Piece type] 2 of N — [what it is for]

[…and so on, in the order they were requested. Exactly the pieces asked for, in the quantities
 asked for. No piece added that was not requested; no piece quietly dropped.]

## 3. Consistency check

| Piece | Core message | The one action | Claim set | Deliberate difference |
|---|---|---|---|---|
| [piece] | ✅ / ⚠️ | ✅ / ⚠️ | ✅ / ⚠️ | [none] or [what differs and why] |

**Where the pieces deliberately differ**

1. **[Piece]** — [what is different] — [the reason: a character limit, a platform convention, a
   channel where the proof point does not fit]

[This section is mandatory and is the one no single-channel skill can produce, because none of them
 sees the other pieces. It must be capable of saying "these two do not agree" — a consistency check
 that only ever confirms everything matches is not a check.]

## 4. Placeholders and gaps

| # | Placeholder | What is needed | Who supplies it |
|---|---|---|---|
| 1 | `[PLACEHOLDER — needs a sourced figure]` | [what claim was wanted and why no bundled file supports it] | [role or team] |

[Every bracketed item in the copy above appears here. If there are none, write "None — every claim
 in this package is sourced to a bundled file." Do not leave the section out.]

## 5. Mapped KR

**[The key result, quoted as it appears in `references/okrs-and-priorities.md`]**

[One or two lines on how this package serves it.]

## 6. SOURCES

- references/[file].md (as of YYYY-MM-DD)
- references/[file].md (as of YYYY-MM-DD) — read in part: [which sections]
- templates/content-package.md (output shape)
- examples/[file].md (standard)
- Corrections: [N entries found in <which file>] | [none found — no corrections file present]

SKILL VERSION: [read it off the line in SKILL.md]

## 7. Next step

[One line. Name the next agent by number and name and offer to hand over.]
```

---

## Rules for filling it in

**Order is fixed.** Core message first, always — it is what every piece is written off, and a
package assembled the other way round is seven pieces that happen to be about the same subject.

**Section 4 is never omitted**, even when it is empty. "None — every claim is sourced" is
information. A missing section reads as an oversight and the reader cannot tell which.

**Every proof-point row names a file.** Not "our research", not "internal data", not "case study" —
the bundled filename. If you cannot name the file, the claim is a `[PLACEHOLDER]`.

**A `[PLACEHOLDER]` stays visibly bracketed in the copy.** Do not write around it, do not soften it
into something vague, and do not quietly drop the sentence that needed it. A vague invented claim is
still invented. Section 4 lists it; the copy shows it.

**Read a file only in part, and say which part.** Write `— read in part: [sections]` in SOURCES. A
judgment resting on a fragment must not look like one resting on the whole file.

**One CTA per piece** (`references/brand-guidelines.md`), and the same action across the package
unless a channel genuinely cannot carry it — in which case that difference is a row in section 3,
not a silent divergence.

**Casing** (`references/brand-guidelines.md`): sentence case for headings, subheadings and body;
Title Case for CTA labels on buttons and links, and for product names. A CTA written as a full
sentence on its own line follows the sentence case of the copy around it and is correct.

**Full product names on first use** — "Zen Planner", not "ZP"; "Daxko Payments", not "Payments".

---

## The partial-package shape — when one conditional file is unusable

If a **conditional** file whose trigger has fired cannot be read — the package names a competitor
and `references/competitive-intel.md` is unreadable, say — you do **not** refuse. You lose part of
one thing, not the package:

- Write every piece that does not depend on it.
- For the part that does, put a `[PLACEHOLDER]` in the copy and a row in section 4 naming the file
  that could not be read.
- Say plainly at the top: **"Partial package — `[filename]` could not be read, so [what is
  affected]."**
- Never guess the part you could not check, and never quietly leave the claim out as though it was
  never wanted.

**A REQUIRED file is different: if one is unusable, you produce no copy at all.** Not a draft, not
one piece, not a partial package. `SKILL.md` step 4 has the exact rule and the one narrow
substitution that is permitted.
