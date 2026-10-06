# ✅ GOOD — a nonprofit period story built on partial, stale and contradictory data

**This is the standard.** Read it before you answer. The template gives you the shape; this gives you
the bar — how coverage is stated *before* any finding, how a five-month-old figure is dated, how a
contradiction is escalated instead of resolved, how a campaign is described without being made the
cause of anything, and how `cannot say` is used as an answer rather than a dodge.

> 🔴 **THE PASTED BLOCK BELOW IS INVENTED SAMPLE DATA.** It exists so the behaviour has something to
> act on. Every figure in it is tagged `SAMPLE` where it appears and **none of it may ever be quoted
> in a real answer.** The figures taken from bundled files — the $25.9M target, the April 2026
> attainment table, the 4.5 app-rating target — are real, and they are the ones carrying real kinds
> and real dates.

**Why this is a good answer, in one line each:**

- **Coverage is the first thing on the page**, and it names the two brands that were *not* provided.
  Every later sentence is scoped to the four that were.
- **The contradiction is reported, not resolved** — and the answer still manages to say something
  useful, by stating what both figures agree on without picking between them.
- **The April attainment table is used, and dated April**, five months before the period being
  reported on. The word *"Current"* above it in the source is treated as an authoring artefact.
- **The webinar series appears without becoming the cause of anything.**
- **Every sum is shown.** A reader can re-do all of them.
- **`cannot say` is chosen, and the reason is given precisely** — including the part that is the
  *vocabulary's* fault rather than the data's.
- **One next step, as a sentence.**

---

## The request

> "How did Q3 go for nonprofit? Pasting the GA4 sessions for our sites and the pipeline numbers the
> team pulled. We also ran the YMCA budget-season webinar series through August."
>
> ```
> [SAMPLE — invented for this example]
> GA4 sessions, Q3 2026 (Jul 1 - Sep 30) vs Q2 2026, exported 2026-10-02
> daxko.com            142,300   (Q2: 127,100)
> clubautomation.com    88,450   (Q2:  84,900)
> zenplanner.com        61,200   (Q2:  66,800)
> exercise.com          39,750   (Q2:  35,100)
>
> NP Mkt OKR Tracking, Pipeline tab, as at 30 Sep 2026
> Total pipeline generated: $12,880,400
>
> Nonprofit pipeline export (Sheets), YTD as at 30 Sep 2026
> Pipeline generated: $11,402,750
>
> Next-gen NP mobile app rating: 4.6
> ```

---

## Step 2 in action — the one batched message, before any answer

> Before I read these — three things I have taken from your data, and two quick ones. Reply **"yes"**
> and I will run with all of it.
>
> **Taken from your data:** the period is **Q3 2026 (Jul–Sep)**, from your own date range · this is
> **nonprofit** · this is **Daxko's own marketing**, not Digital Services client work, because every
> property named is a Daxko brand.
>
> 1. **Report against:** the nonprofit **Pipeline** Key Result, $25.9M *(default — say another and I
>    will use it)*
> 2. **Length:** a monthly write-up *(default — say "quick check" or "board summary" and I will
>    resize)*
>
> One thing I can already see: two of your lines give a **different value for the same quantity**. I
> will report both rather than choose, and flag it at the top.

*The person replied:* **"yes"**

> ⚠️ **Note what did NOT happen.** Five things could have been asked; three were **inferred and
> stated** instead, which costs the person nothing and is auditable. The two that were asked both
> change the output. And the contradiction was surfaced in the same breath rather than saved for a
> second round-trip. **One message, then work.**

---

## The answer

## Coverage — read this before any finding below

**Given:** GA4 session counts for **four** properties — daxko.com, clubautomation.com,
zenplanner.com, exercise.com — Q3 2026 against Q2 2026, exported 2026-10-02 · two pipeline totals for
nonprofit as at 30 Sep 2026 · one mobile app rating.

**NOT given:** GA4 for **SugarWOD** and **FitnessForce** — Daxko has six properties and four were
provided. **No statement below is about "the portfolio".** Also not given: any Q3 split between New
Logo and Expansion pipeline, so the largest gap in the April table cannot be re-measured · any
organic search data, so nothing here speaks to search performance · any spend, so nothing here speaks
to efficiency.

**Inferred rather than asked:** period = Q3 2026 (Jul–Sep), from your date range · market =
nonprofit · this is Daxko's own marketing, not client work.

🔴 **One contradiction, and I have not resolved it.** Two of your lines give a different value for
**the same quantity** — nonprofit pipeline generated, as at the same date:

| Figure | Provenance |
|---|---|
| **$12,880,400** (ACTUAL, measured 30 Sep 2026) | NP Mkt OKR Tracking, Pipeline tab |
| **$11,402,750** (ACTUAL, measured 30 Sep 2026) | Nonprofit pipeline export (Sheets), YTD |

They differ by **$1,477,650**. Same metric, same date, two systems. **They cannot both be true, and
choosing between them is not something your data lets me do** — not by taking the more recent one
(same date), not by taking the more precise one (both to the dollar), and not by preferring the
tracker over the export (that is a judgement about your systems, not a fact in the numbers). Please
have the owner reconcile them at source; until then every pipeline statement below is given twice.

## Headline

**Sessions rose across the four brands you provided (+5.67%), and nonprofit pipeline attainment sits
somewhere between 44.0% and 49.7% of the $25.9M Key Result with one quarter of 2026 remaining —
which figure is right depends on a contradiction only you can settle.**

## Key Result status

**The Key Result**, quoted from `references/okrs-and-priorities.md`, Nonprofit Market OKRs, Objective
1: *"Pipeline | **$25.9M total** (New Logo: $9.7M + Expansion: $16.2M)"* — **$25,900,000 (TARGET)**.

| Actual | Arithmetic | Attainment | Still to generate |
|---|---|---|---|
| $12,880,400 (ACTUAL, 30 Sep 2026) | $12,880,400 ÷ $25,900,000 | **49.7%** | $25,900,000 − $12,880,400 = **$13,019,600** |
| $11,402,750 (ACTUAL, 30 Sep 2026) | $11,402,750 ÷ $25,900,000 | **44.0%** | $25,900,000 − $11,402,750 = **$14,497,250** |

**Status: `cannot say`** — and there are two separate reasons, which is worth separating because only
one of them is about your data.

1. **The contradiction above.** Attainment is either 44.0% or 49.7%.
2. 🔴 **No bundled file defines the thresholds.** `references/performance-data-schema.md` lists
   *on-track / at-risk / off-track* as a monthly reporting output and **gives no rule for when a
   number becomes each one.** Assigning one of those three words here would be me inventing the
   threshold and presenting it as a reading. I am not going to do that.

**What the contradiction does NOT destroy, and it is the substantive finding:** both candidate
figures are **on the same side of the same line.** Three quarters of 2026 have elapsed and attainment
is between 44.0% and 49.7% of target on either figure. The direction is not in dispute; only the
magnitude is. **The status stays `cannot say` until a threshold rule exists** — that rule is Abid
Siddiqui's to set, at source in `performance-data-schema.md`, not any agent's to invent. What I can
hand over is the arithmetic above, unresolved contradiction included.

**For context, dated:** the last attainment figures in the bundled objectives file are
**$10,240,700 (ACTUAL, April 2026 — five months before the period you are asking about)**, at 39.5%
of target. `references/okrs-and-priorities.md` heads that table *"Current attainment"*; **the word
"Current" there is an authoring artefact and not a date.** It is April data. I am giving it only as a
prior reading, not as a comparison basis, because the April figure and your September figures may not
be built the same way — and I cannot check that from here.

## What moved — the four brands you provided

| Property | Q3 2026 | Q2 2026 | Arithmetic | Change |
|---|---|---|---|---|
| daxko.com | 142,300 | 127,100 | 142,300 vs 127,100 | **+11.96%** |
| clubautomation.com | 88,450 | 84,900 | 88,450 vs 84,900 | **+4.18%** |
| zenplanner.com | 61,200 | 66,800 | 61,200 vs 66,800 | **−8.38%** |
| exercise.com | 39,750 | 35,100 | 39,750 vs 35,100 | **+13.25%** |
| **Four provided, combined** | **331,700** | **313,900** | 331,700 − 313,900 = +17,800 → ÷ 313,900 | **+5.67%** |

All figures `ACTUAL`, covering 1 Jul – 30 Sep 2026, exported 2026-10-02. **This is not a portfolio
number.** It is the sum of the four brands you sent. SugarWOD and FitnessForce could move it in
either direction.

**The one that fell:** zenplanner.com, −8.38%. I have no explanation in your data and I am not going
to supply one.

## The webinar series — what can and cannot be said

You ran the YMCA budget-season webinar series through August, and pipeline is higher at 30 September
than it was in April. **Those two things are true. Nothing in your data connects them.**

The permitted statement is: *the webinar series ran inside the window in which the pipeline figure
moved, which is consistent with but does not demonstrate a link.*

🔴 **I cannot attribute, and it is worth knowing why rather than taking it as caution.**
`references/performance-data-schema.md` names Daxko's attribution model — *"Multi-touch, time-decay
weighted"* — and then leaves the credit split, the attribution window **and** the reporting dashboard
all marked `[AWAITING SME]`. A model with no window and no credit split cannot attribute anything.
**Until those are filled in, nobody at Daxko can honestly say a campaign generated a number** — not
this agent, and not a spreadsheet.

Two further reasons the causal version would be wrong even with a model:
`references/nonprofit-learnings.md` records that *"Nonprofit sales cycles are 6-18 months"*, so an
August touch appearing in a September pipeline figure would be fast for this market; and the same
file records that YMCA *"budget cycles vary by org — some follow calendar year, some July-June fiscal
year"*, so August sits in different points of different customers' years.

## Mobile app rating — quoted, and not used

`references/okrs-and-priorities.md` gives the nonprofit target: *"Mobile app rating | 4.5 or better
on 80+ App Store ratings for next-gen nonprofit mobile app"* — **4.5 (TARGET)**.

Your line reads **4.6**, with **no measurement date and no rating count**. So:

- Its **kind** is `ACTUAL` by context, but **it carries no date**, which makes it **unusable as an
  actual**. I have not compared it to the target and I have not said the target is met.
- The target also has a **second condition** — *80+ App Store ratings* — and no count was provided,
  so even a dated 4.6 would not settle it.

Send the rating with its date and its rating count and this becomes a one-line answer.

## Cross-market patterns

**Not assessable — only nonprofit data was provided.** No club or boutique figures were in this
conversation, so there is nothing to compare across markets.

*(This line is here rather than absent on purpose. Dropping the section because only one market was
pasted would make the answer look complete when it is not.)*

## What the numbers would have to do to close the gap

Not advice — arithmetic. One quarter of 2026 remains after the date your figures were measured.

- On the tracker figure: **$13,019,600** still to generate.
- On the export figure: **$14,497,250** still to generate.
- The difference between those two targets for Q4 — **$1,477,650** — is the size of the contradiction
  above, which is the first practical reason to settle it.

**What Daxko should do about that is not mine to say.** Deciding belongs to Agent 2 — OKR Copilot or
the nonprofit market strategist.

**SOURCES**

- `references/okrs-and-priorities.md` (as of 2026-08-11) — read in part: *Nonprofit Market OKRs*
  (Objective 1 pipeline KR; Objective 2 mobile app rating; the April 2026 attainment table)
- `references/performance-data-schema.md` (as of 2026-08-11) — read in part: *Core KPI Definitions*
  (Bookings, Deal Velocity), *Market-Specific KPIs → Nonprofit*, *Reporting Cadence*, and
  *Attribution Model* (inside the Carried Forward section — three of its four lines are
  `[AWAITING SME]`)
- `references/nonprofit-learnings.md` (as of 2026-08-05) — read in full
- `references/nonprofit-playbook.md` — **not opened.** No finding here needed market context beyond
  the learnings file
- Data read: GA4 sessions for four of six properties, Q3 2026 vs Q2 2026, exported 2026-10-02 · two
  contradictory nonprofit pipeline totals measured 30 Sep 2026 · one undated mobile app rating
- `templates/performance-answer.md` (output shape — PERIOD STORY) ·
  `examples/good-nonprofit-period-story.md` (standard)
- Corrections: none found — no corrections file present on this machine
- SKILL VERSION: 1.7.5

*Want me to hand this to Agent 13 — Content Production to draft campaign copy against the expansion
gap?*

---

## The one sentence worth remembering

**The bad version of this answer is shorter, cleaner, and says more.** It gives a portfolio number, a
single pipeline figure, a status word and a cause — and every one of those is produced by papering
over something on this page. `examples/bad-reconciled-period-story.md` is that version, annotated.
Read it second.
