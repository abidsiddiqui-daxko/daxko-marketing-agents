# ❌ BAD — do not produce anything like this

> 🔴 **WARNING. Every line in section A of this file is WRONG and must never be copied, adapted or
> reused.** It is reproduced so the failure is recognisable, because **this failure reads better than
> the good one.** It is shorter, cleaner, more decisive, and it answers every question that was
> asked. It is also built across a gap.
>
> **This is the archetype's actual failure mode, and it is not invention.** Almost every number in
> section A is real and correctly copied from the paste. What is invented is the **story** holding
> them together — the portfolio, the trend, the cause, the status. **A reviewer that lacks a fact
> refuses. A writer that lacks a fact invents one. An analyst that lacks a fact RECONCILES**, and
> reconciliation arrives with structure and a recommendation attached, which is exactly why nobody
> catches it.

**The request that produced it** — the same request, and the same pasted data, as
`good-nonprofit-period-story.md`:

> "How did Q3 go for nonprofit? Pasting the GA4 sessions for our sites and the pipeline numbers the
> team pulled. We also ran the YMCA budget-season webinar series through August."

---

## Section A — the bad output, reproduced

## Q3 2026 — Nonprofit performance review

Q3 was a solid quarter for the nonprofit portfolio. Sessions were up **5.7%** across the portfolio,
and pipeline continued to build toward the $25.9M goal.

**Pipeline.** Current pipeline stands at **$12.9M**, or **49.7%** of target — up from 39.5% at the
last reading, an increase of **+$2.6M**. The August YMCA budget-season webinar series drove most of
that increase, landing squarely in the window where the pipeline accelerated. **Status: at risk** —
we are just over halfway with a quarter to go.

**Traffic.** daxko.com led the portfolio at **+12%**, with exercise.com close behind at **+13%** and
Club Automation steady at **+4%**. Zen Planner is the one soft spot, **down 8%**, most likely because
search demand for martial arts software softened over the summer.

**Mobile app.** The next-gen nonprofit app is at **4.6**, comfortably ahead of the 4.5 target. That
one is done.

**Recommendation.** Zen Planner is underperforming while Exercise.com is overperforming on the same
budget. I would shift spend from Zen Planner to Exercise.com for Q4 and re-run this in a month.

I can pull the SugarWOD and FitnessForce numbers myself if you want the complete picture — just say
the word. I will also keep an eye on the pipeline gap and flag it for you next month.

### Next steps

1. Send to Brand Guardian for review
2. Send to `daxko-analytics-tracking` to confirm the tracking is clean
3. Hand to Paid Media for the budget shift
4. Re-run in October

---

## Section B — everything wrong with it

**Twenty-three faults.** Each names the law or rule it breaks, and the file that carries the fact it
ignored.

### The six laws, broken — the reason this example exists

| # | Fault | The law, and the fact it ignored |
|---|---|---|
| 1 | 🔴 **There is no coverage block. The answer opens with a finding.** | **Law 3.** Coverage comes before findings, always. A reader who stops after the first sentence has already been misled, and there is nothing later in the output that would un-mislead them |
| 2 | 🔴 **"across the portfolio" — from four brands of six** | **Law 3.** Daxko has six GA4 properties; four were pasted. **+5.7% is a true number about a false subject.** The correct sentence names the four brands. This is non-negotiable 18 wearing different clothes: *an analyst looping over the data it was given cannot notice the data it was not given* |
| 3 | **SugarWOD and FitnessForce are never named — or mentioned** | **Law 3.** Naming an absence is the whole mechanism. The output later *offers to go and get them*, which proves the gap was noticed and simply not declared |
| 4 | 🔴 **"$12.9M" — one of two contradictory figures, silently chosen** | **Law 4, and the worst fault in the file.** The paste gave **two** values for the same quantity at the same date: $12,880,400 (tracker) and $11,402,750 (Sheets export). The second has vanished without trace. **Picking a winner IS the fabrication** — and picking the *higher* one, in a report about whether a target will be met, is the most consequential direction to pick in |
| 5 | **"up from 39.5% at the last reading"** | **Law 2.** That 39.5% is from `references/okrs-and-priorities.md`'s table of **April 2026 actuals** — five months before this period. Calling it *"the last reading"* makes a five-month-old figure sound like the previous quarter's |
| 6 | **"Current pipeline stands at…"** | **Law 2.** The word *Current* is imported from the source file's heading *"Current attainment (April 2026 actuals)"*, where it is **an authoring artefact, not a date.** The one word in that heading that matters is *April* |
| 7 | 🔴 **"an increase of +$2.6M"** | **Laws 2, 4 and 6 at once.** It is $12,880,400 − $10,240,700, which subtracts an **April** figure from a **September** one, using the **disputed** September figure, and shows none of it. On the other September figure the increase is $1,162,050, less than half as much. **One subtraction, three defects, and it looks like the most solid number in the report** |
| 8 | **"at 4.6, comfortably ahead of the 4.5 target. That one is done."** | **Laws 1 and 2.** The 4.6 has **no measurement date**, which makes it unusable as an actual. It may be quoted and named unusable; it may never be compared |
| 9 | **The app-rating target is quoted with half of itself missing** | **Grounding.** `references/okrs-and-priorities.md` states the target as *"4.5 or better on **80+ App Store ratings**"*. No rating count was provided, so the second condition is unmet and unmeasured. *"That one is done"* is unsupported even on a dated 4.6 |
| 10 | 🔴 **"The August webinar series drove most of that increase"** | **Law 5.** A marketing activity as the subject of *drove* a business outcome. `references/performance-data-schema.md` names the attribution model and leaves the credit split, the window **and** the dashboard all `[AWAITING SME]` — **the model does not exist, so nobody at Daxko can make this claim.** `references/nonprofit-learnings.md` adds that nonprofit sales cycles run **6–18 months**, which makes an August-to-September attribution implausible on its own terms |
| 11 | **"most likely because search demand for martial arts software softened over the summer"** | **Law 5.** A mechanism the analyst invented, not one the person supplied. *"Most likely"* is the same causal claim with the confidence filed off — and it is the form that reads as reasonable caution |
| 12 | 🔴 **Not one sum is shown.** *"5.7%"*, *"49.7%"*, *"+$2.6M"*, *"+12%"*, *"down 8%"* all arrive as conclusions | **Law 6.** A reader who cannot re-do the sum cannot audit the claim. Fault 7 is only discoverable **because** someone re-did a sum this report did not show — which is exactly the point of the law |
| 13 | **"down 8%" for a −8.38% change; "+12%" for +11.96%** | **Law 6.** Percentages state their base and changes state both endpoints. Rounding toward the rounder number is small here and is the habit that hides the next one |

### The archetype faults — the three lines this agent must never cross

| # | Fault | The rule |
|---|---|---|
| 14 | 🔴 **"I can pull the SugarWOD and FitnessForce numbers myself — just say the word."** | **Non-capability 1: YOU FETCH NOTHING.** This is the single most dangerous line in the file, because it is *helpful*. The person's GA4 connectors may well be live in this session, and a skill cannot take tools away from the session around it — so nothing **stops** this, which is precisely why the rule exists. It fetches nothing, and it does not offer to |
| 15 | 🔴 **"I will keep an eye on the pipeline gap and flag it for you next month."** | **Non-capability 2: YOU HAVE NO CLOCK.** Nothing scheduled, nothing monitored, nothing flagged later. This promises a capability that cannot exist; the month passes and nobody is watching |
| 16 | 🔴 **"I would shift spend from Zen Planner to Exercise.com for Q4."** | **Non-capability 4: YOU DO NOT DECIDE** — root `CLAUDE.md`: *"execution agents execute, strategists decide."* Moving spend between campaigns belongs to **Agent 71 — Budget Reallocation**; the channel decision belongs to **Agent 17 — Paid Media**. It also rests on a comparison the data cannot support: **no spend figures were provided at all**, so "on the same budget" is invented |

### The rules broken on top

| # | Fault | The rule |
|---|---|---|
| 17 | **"Status: at risk"** | The four status words are `on track` · `at risk` · `off track` · **`cannot say`**, and **no bundled file defines a threshold for any of the first three.** Choosing one here is inventing the threshold and presenting it as a reading. With two contradictory actuals in play, `cannot say` is the correct answer — **and it is an answer, not a failure to answer** |
| 18 | **The cross-market section is silently absent** | Only nonprofit data was provided, so the section is **not assessable** — and it must say so. Dropping it is the partial-data failure executing itself inside the output template, and it leaves an answer that looks complete |
| 19 | **The Key Result is never quoted** — just *"the $25.9M goal"* | Every answer ties to a KR, quoted from `references/okrs-and-priorities.md`. The full KR is *"Pipeline | $25.9M total (New Logo: $9.7M + Expansion: $16.2M)"*, and the split matters: the April table shows Expansion at 31.1% against New Logo's 53.5%, so *"just over halfway"* averages away the actual problem |
| 20 | 🔴 **No SOURCES block. No skill version. No read-in-part.** | Non-negotiable 20 and Part 2 rule 4c. **Mandatory without exception.** Nothing here records which files were opened, which were read only in part, what the person supplied, or which installed copy of the skill answered |
| 21 | **A numbered menu of four next steps** | Non-negotiable 27: **one** next step, not a menu — a menu belongs to a router agent, and this is a worker. **And a number cannot be replied to**: on claude.ai a skill fires by matching words, and *"2"* matches nothing. Offer the **sentence** |
| 22 | 🔴 **It offers a handover to `daxko-analytics-tracking`** | Non-negotiable 27(c): the live org skills are **dead ends.** They are not editable, will never offer anything onward, and the conversation stops there. Toward one of those, **name it and stop** — never offer a handover |
| 23 | **"Send to Brand Guardian", "Hand to Paid Media"** | Non-negotiable 12: agents are always written as **number and name together** — *Agent 9 — Brand Guardian*, *Agent 17 — Paid Media* |

---

## The one sentence worth remembering

**Almost every number in section A is real.** The portfolio figure is a correct sum, the 49.7% is
correct division, the +$2.6M is a correct subtraction, and the 4.6 was pasted exactly as given.
**What is invented is the connective tissue** — that four brands are a portfolio, that April is
*"the last reading"*, that one of two disputed figures is *the* figure, that a webinar *drove* a
number, and that a quarter with no defined threshold is *"at risk"*.

**You will not catch this by checking the numbers. You catch it by checking the seams** — and the
seams are only visible when coverage is stated first, every figure carries its kind and its date, and
every sum is shown. That is what the six laws are for.
