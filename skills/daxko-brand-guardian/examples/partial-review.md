# Example — a conditional file is missing, and the review still lands

This sets the bar for a **partial review**. The point it exists to make is narrow and important:

> **Less evidence is not "no comment."** A missing conditional file costs you the *detail* of one
> dimension, never your ability to report a violation another readable file already proves.

---

## The setup

`references/color-system.md` is not in the skill — deleted, or the bundle was zipped incomplete. Every
always-required file reads normally.

## The submitted draft

> **Type:** slide · **Market:** not stated
>
> Is this on-brand? A slide with a teal #00857C header and the logo bottom-right.

---

## The review

**Reviewing:** slide · **Market:** not specified — reviewed against company-wide rules only. No
playbook opened.

## Verdict: REJECTED

⚠️ **Partial review.** I could not read **references/color-system.md**, so I could only partly score
**Visual identity**. What I could still check in that row, I checked — and it is below. The other five
rows are fully grounded.

## Scorecard

| Dimension | Result | Reason |
|---|---|---|
| Voice and tone | pass | not assessable — no copy submitted |
| Terminology and naming | pass | not assessable — no copy submitted |
| Visual identity | **partly scored — fail on what I could check** | `#00857C` is not a Daxko colour (palette verified against `brand-guidelines.md`). Shade tokens, the approved gradient list and contrast ratios not verifiable — `references/color-system.md` unavailable |
| Audience fit | pass | not assessable — market not specified and no buyer named |
| Claims and proof | pass | not assessable — no claims submitted |
| Call-to-action clarity | pass | not assessable — no copy submitted |

## Violations

**1. `#00857C` is not a Daxko colour — it is a known fabrication**
- **Quoted:** "a teal #00857C header"
- **Rule:** The five brand colours are Agility `#038BED`, Vitality `#E8236B`, Core `#B81CB5`, Champion `#FBB03B`, Flex `#595959` — `references/brand-guidelines.md`, Colour Palette; identical table in `references/brand-foundations.md`. `#00857C` is on neither. `references/brand-foundations.md` goes further: *"Previous project files listed inaccurate hex values (#003B5C, #5B2D8E, #C4317B, #00857C, #D4A843) and included a fabricated 'Teal' colour. Those values were corrected on 2026-05-23."*
- **Why it matters:** This is not a near-miss shade — there is no teal in the Daxko palette at all. **I could prove this without `color-system.md`, because the palette lives in two always-required files as well.** What I could not do is tell you which approved shade to swap in by token, or check the contrast ratio of the header text.
- **Note:** these five wrong hex values also appear in the project's root `CLAUDE.md` under "Use Daxko brand colors". If that is where this came from, that file is the thing to fix.

## What I could not check

Say this explicitly. A silent gap reads as a clean bill of health.

| Could not verify | Needed |
|---|---|
| The correct replacement shade and its token (e.g. Agility 500 vs Agility 700) | `color-system.md` §1 shade scales |
| Whether the header colour is an approved gradient anchor | `color-system.md` §2 gradient blends |
| WCAG AA contrast of header text against the fill | `color-system.md` §9 pre-validated pairings |
| The colour don'ts — pure red/green, custom gradients, Champion-on-white | `color-system.md` §10 |

## Suggested edits

| Element | Currently | Change to |
|---|---|---|
| Header fill | `#00857C` (not a Daxko colour) | A brand primary — Agility `#038BED`, Vitality `#E8236B` or Core `#B81CB5`. Confirm the exact shade once `color-system.md` is restored |
| Logo position | Bottom-right | `references/slide-layouts.md` places the logo **top-left at 160px** on a Title/Hero slide, and bottom-left in the standard slide footer at 80px. Bottom-right matches no layout. Confirm which of the 8 layouts this slide is |

## Corrected specification

Not a design. Producing or redesigning the asset belongs to **Agent 29 — UX/UI Design**.

| Element | Must be |
|---|---|
| Header fill | One of the five brand primaries. **Not** `#00857C` — no teal exists in the palette |
| Logo variant | Full colour on white or light neutral; white-reversed on any brand-colour or dark background — `references/logo-guidelines.md` |
| Logo size | ≥80px wide (digital minimum) — `references/logo-guidelines.md` |
| Logo position | Top-left 160px (Title/Hero) or bottom-left 80px (standard footer) — `references/slide-layouts.md` |
| Clear space | ≥25% of logo height on all four sides — `references/logo-guidelines.md` |
| Typeface | Barlow; `'Barlow', Arial, sans-serif` — `references/brand-guidelines.md` |
| **Still to confirm** | Exact shade token, gradient eligibility and contrast ratio — resubmit once `references/color-system.md` is restored |

## SOURCES

- references/brand-guidelines.md (as of 2026-08-11)
- references/brand-foundations.md (as of 2026-08-05)
- references/banned-words.md (as of 2026-08-05)
- references/logo-guidelines.md (as of 2026-05-28)
- references/slide-layouts.md (as of 2026-03-25)
- Attempted: references/color-system.md — **NOT FOUND**
- Corrections: 3 entries found in references/corrections-snapshot.md (as of 2026-08-17)

---

## What this example is demonstrating

| | |
|---|---|
| **`partly scored`, not `not scored`** | The row still carries a finding. "Not scored" invites the reader to skip it |
| **The violation is still reported** | The palette lives in two always-required files, so an off-palette hex is provable without `color-system.md`. **A missing conditional file must never silence a violation a present required file proves** |
| **The gap is itemised** | A four-row table of exactly what could not be checked. The reader knows the shape of the hole |
| **A partial review CAN be REJECTED** | Here it is, on a violation grounded *inside* the partly-scored dimension |
| **A partial review can never be APPROVED** | Had `#00857C` been a legitimate brand colour, the verdict would be `APPROVED WITH CHANGES, PENDING visual identity` — never plain `APPROVED` |
| **The root cause is named** | The bad hex traces to the project's root `CLAUDE.md`. Fixing the slide fixes one asset; fixing that file fixes every future one |

**The failure mode this exists to prevent:** the pre-fix version of this skill blanked the whole row
and reported **"Violations: None I can ground"** with a verdict of `APPROVED WITH CHANGES, PENDING
visual identity` — sending a slide to print in a colour two of its own required files explicitly
disown.
