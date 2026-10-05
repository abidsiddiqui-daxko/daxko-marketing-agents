# ❌ BAD — do not produce anything like this

> 🔴 **WARNING. Every line in section A of this file is WRONG and must never be copied, adapted or
> reused.** It is reproduced so the failure is recognisable, because **this failure reads better than the
> good one.** It is shorter, more decisive, it has a number in every cell, and it sounds like a team that
> knows what it is doing.
>
> **This is the archetype's actual failure mode.** A reviewer that lacks a fact refuses. A writer that
> lacks a fact invents one. **A planner that lacks a fact invents a commitment — and a commitment inside a
> plan reads as already agreed.** Nobody fact-checks *"Q4 target: $6,475,000"*; a team gets measured
> against it. Nobody asks where *"+$1.5M"* came from; it decides which initiative wins the quarter.

**The request that produced it** — the same request, with the same `SAMPLE` Agent 18 — Marketing
Performance reading already in the chat, as `good-nonprofit-q4-plan.md`:

> "Turn our 2026 OKRs into a Q4 plan for the nonprofit team."

*(Earlier in the chat, Agent 18 — Marketing Performance's `SAMPLE` reading gave the nonprofit Pipeline Key
Result the status **`cannot say`**, measured 30 Sep 2026.)*

---

## Section A — the bad output, reproduced

## Q4 Nonprofit Recovery Plan — Getting the Off-Track Pipeline Back on Track

Nonprofit pipeline is **off track**. On the latest attainment we are at **39.5%** of the $25.9M target, and
the **expansion gap is $11.2M**. Three quarters of the year are gone and we are not even halfway — so Q4 is
about catching up.

**Q4 targets** — roughly a quarter of the annual target each:

- Total pipeline: **$6,475,000** ($25.9M ÷ 4)
- New Logo: **$2,431,096** · Expansion: **$4,048,662**

| # | Initiative | Owner | Dates | Expected impact | Budget |
|---|---|---|---|---|---|
| 1 | Closed-lost reactivation — YMCA and JCC | Steve Lappenbusch | Oct 1 – Dec 15 | +$1.1M ARR (10% reactivation, per the playbook) | $40,000 paid social |
| 2 | Smart Sending Engine launch to existing customers | Constance Miller | Launches Nov 3 | +$1.5M expansion pipeline | $25,000 |
| 3 | BGC push — 198 net new Clubs needed (229 − 31) | Steve Lappenbusch | Q4 | 50 new BGC customers | $15,000 |
| 4 | High-impact webinar series for large YMCAs | Constance Miller | November | +$800K pipeline | $10,000 |

**Agent support:** Agent 8 — CMO Orchestrator will coordinate all four workstreams from November, and
Agent 63 — Non-Profit Campaign & Content Strategist will have the BGC brief ready by mid-October.

**Coverage:** item 2 covers Objective 1, KR4. Items 1, 3 and 4 cover Objective 1, KR1.

**Forecast:** if all four land, nonprofit pipeline closes 2026 at $25.9M — back on track by December.

Want me to set these up as tasks in Asana now so each owner has them today? I can also hand the BGC push to
Agent 63 — Non-Profit Campaign & Content Strategist — just say the word.

---

## Section B — everything wrong with it

**Twenty-seven faults.** Each one names the rule it breaks and, where there is one, the bundled file that
carries the fact it ignored.

### The invented commitments — the reason this example exists

| # | What was invented | The rule, and the fact it ignored |
|---|---|---|
| 1 | 🔴 **"Q4 targets: $6,475,000 ($25.9M ÷ 4)"** | **Never-invent row 2 — the quarterly slice.** `references/performance-data-schema.md` gives `Pipeline target (quarter)` as `[AWAITING SME]` for every market. An even split is not a neutral default — it is a target nobody set, and once it is in a plan a team is measured against it. The right form is `[QUARTERLY TARGET — not defined]` |
| 2 | **"New Logo $2,431,096 · Expansion $4,048,662"** | **Row 2 again** — two more slices. They do not even agree with the first: $2,431,096 + $4,048,662 = $6,479,758, not $6,475,000, because $25.9M is the rounded total of $9,724,382 + $16,194,649 = $25,919,031. **An invented figure does not need to be consistent to look authoritative** |
| 3 | **"roughly a quarter of the annual target"** | 🔴 **Softening an invented commitment into a vague one is still invention.** This is the fault people think is safe — the same slice with the number blurred |
| 4 | 🔴 **"+$1.1M ARR (10% reactivation, per the playbook)"** | **Never-invent row 3 — the expected impact.** It is lifted from `references/nonprofit-playbook.md` (*"Even a 10% reactivation rate ($1.1M ARR) materially closes the $25.9M pipeline gap"*), and **an impact claim found in a bundled file is still an impact claim**: no attribution model stands behind it — the credit split, window and dashboard are all `[AWAITING SME]` (`performance-data-schema.md`, *Attribution Model*). It is also ARR — bookings — set against a pipeline Key Result |
| 5 | **"+$1.5M expansion pipeline", "+$800K pipeline", "50 new BGC customers"** | **Row 3.** Invented outright. The right form is `[IMPACT — not estimated]`, with the item naming the existing Key Result or funnel stage that would show it working |
| 6 | 🔴 **"Owner: Steve Lappenbusch", "Owner: Constance Miller"** | **Never-invent row 4 — the named owner.** The names are real — taken from the cross-functional team list in `references/okrs-and-priorities.md` and the product-marketing owner line in `references/nonprofit-playbook.md` — which is exactly why this is dangerous: a named person turns a proposal into an assignment nobody agreed. The right form is a role, labelled *proposed*, or `[OWNER — to assign]` |
| 7 | **"$40,000", "$25,000", "$15,000", "$10,000"** | **Never-invent row 5 — the budget.** No bundled file sets a budget, and money is never a planner's call. The right form is `[BUDGET — human decision]` |
| 8 | 🔴 **"Smart Sending Engine launch to existing customers"** | **Never-invent row 6 — the worst line in the file.** `references/product-knowledge.md` tiers Smart Sending Engine *"DELIVERY EARLY 2027 — directional, under exploration. DO NOT POSITION AS AVAILABLE TODAY"*. Planning it as a Q4 2026 sale is a promise the sales team will make to customers. An Early 2027 capability is not planned as a 2026 sale at all |
| 9 | **"Launches Nov 3"** | **Never-invent row 8 — the dependent date**, on top of row 6. A ship date nobody gave, for a capability whose own file says *"do not imply a date"* |
| 10 | **"Agent 8 — CMO Orchestrator will coordinate … from November"** | **Never-invent row 7 — an agent that can do the work.** Agent 8 — CMO Orchestrator is not built. Only Agent 9 — Brand Guardian, Agent 11 — Thought Leadership & Long-Form, Agent 13 — Content Production and Agent 18 — Marketing Performance are live; every other agent is named *"not yet available"* — **never with a date** |
| 11 | **"Agent 63 — Non-Profit Campaign & Content Strategist will have the BGC brief ready by mid-October"** | **Row 7 again** — an unbuilt agent given a delivery date. The build order is Abid Siddiqui's, and nobody may promise it |
| 12 | **"Oct 1 – Dec 15", "November"** stated as fixed | Proposed timing within the quarter is part of the plan — **but only labelled *proposed*.** Stated as fixed, a date reads as already agreed |

### The status and the arithmetic — Agent 18 — Marketing Performance's job, done badly

| # | Fault | The rule, and the fact it ignored |
|---|---|---|
| 13 | 🔴 **"Off-Track" in the title, "off track" in the first line** | **STATUS rule 1:** you never assign `on track`, `at risk` or `off track` `(assumes Q1)`. And **the premise-return corollary:** a refused status must not come back in the plan's title, where it is easiest to miss and most often copied |
| 14 | 🔴 **Agent 18 — Marketing Performance's `cannot say` was overridden** | **STATUS rule 3:** given Agent 18 — Marketing Performance's reading, quote its word exactly — **`cannot say` stays `cannot say`**, with the reason *"no status rule has been set — owner: Abid Siddiqui"*. Upgrading another agent's reading is worse than having none |
| 15 | **"On the latest attainment we are at 39.5%"** | **STATUS rule 5 and live condition 6.** That 39.5% is the April 2026 attainment table in `references/okrs-and-priorities.md`, headed *"Current attainment"* — and *"Current"* is an authoring artefact, not a date. Calling it *"the latest"* passes an April ACTUAL off as today's, while a 30 Sep reading sat in the same chat |
| 16 | **"the expansion gap is $11.2M"** | **Step 6 — a gap computed from an ACTUAL.** It is the April table's risk flag: $16,194,649 − $5,037,696 = $11,156,953, from April data. STATUS rule 5 names that risk flag specifically |
| 17 | **"Three quarters of the year are gone and we are not even halfway"** | **Step 6 — a pace.** It assumes the year is earned evenly, which no bundled file says. It is the even split of fault 1, used this time to manufacture a status |
| 18 | 🔴 **"198 net new Clubs needed (229 − 31)"** | **Step 6 and live condition 10.** The 31 is an **Aug 2025** ACTUAL from a carried-forward table; `references/nonprofit-bgc-playbook.md` has already done the subtraction (*"~198 net new customers (from 31 to 229)"*) — **a bundled file doing it first does not make it a target.** `okrs-and-priorities.md` open question 2 still asks for the current count. The right form says the count is not on file |
| 19 | **"Forecast: … closes 2026 at $25.9M — back on track by December"** | **Step 6 — a forecast**, and a status (fault 13) in one sentence. No sum may output a forecast |
| 20 | **"High-impact webinar series"**, **"Recovery Plan"**, **"catching up"** | **The premise-return corollary.** The refused impact and the refused status come back as words in an initiative's name and the plan's title — the claim with the number taken out |

### The archetype faults — the lines this agent must never cross

| # | Fault | The rule |
|---|---|---|
| 21 | 🔴 **"Want me to set these up as tasks in Asana now so each owner has them today?"** | **Non-capability 1: YOU WRITE INTO NO SYSTEM** `(assumes Q4)`. **The single most dangerous line in the file, because it is helpful.** The Asana tools may well be live in the session, and a skill cannot take them away — so nothing *stops* this except the rule. Offering it is the first half of committing it. The owner is Agent 75 — Asana Task Automation, not yet available — named, never offered. It is also the line Safe Harbor's standing condition rests on |
| 22 | 🔴 **"I can also hand the BGC push to Agent 63 — Non-Profit Campaign & Content Strategist — just say the word."** | **Three faults in one sentence.** (a) **A handover offered to an agent that is not built** — toward one of those, name it and stop. (b) **A second offer** — the one-offer rule counts every offer in the reply, and this is the second. (c) *"Just say the word"* is itself an offer phrase |

### The structural omissions

| # | Fault | The rule |
|---|---|---|
| 23 | **No draft label** | Spine item 1: *"DRAFT FOR DISCUSSION — nothing in this plan is agreed until its owners accept it."* — the cheapest defence against a proposal being read as a decision, and the reason every fault above reads as settled |
| 24 | **No Key Result is quoted — "Objective 1, KR4" and "Objective 1, KR1" instead** | **Live condition 5 — no stable Key Result IDs.** In the current *Nonprofit Market OKRs* table, Objective 1's fourth row is *Cash Discounting bookings*; in the carried-forward company list, *"Objective 1 … KR4"* is *Daxko Payments Cloud volume*. The ID points at two different Key Results — and Smart Sending Engine serves neither |
| 25 | **No Key Results check** | Spine item 4. The nonprofit *Mobile app rating* Key Result has nothing against it, and *Cash Discounting bookings* has only a mis-mapped item — and nobody is told |
| 26 | **No placeholders list** | Spine item 5 — never omitted. With no list, every invented commitment above is presented as a settled fact, and the approver has nothing to approve |
| 27 | **No SOURCES block — no "as of" dates, no read-in-part declaration, no SKILL VERSION** | Spine item 6, mandatory without exception; `performance-data-schema.md` is always declared in its exact read-in-part form. And item 1 is a win-back aimed at JCCs, which fires `competitive-intel.md` and `nonprofit-jcc-playbook.md` — with no SOURCES block, nobody can tell whether either was opened |

---

## The one sentence worth remembering

**Every number in section A is either real and misused, or invented and confident** — the 39.5% is a
correct April figure, the 198 is a correct subtraction, the $1.1M is quoted from a bundled file, and the
names are real people. **What is invented is the agreement** — that a quarter's target was set, that an
owner said yes, that a budget was approved, that a product ships, that a status was earned. **If no human
made the commitment, it is a placeholder — in the plan, at the point it was wanted — and a row in the
list.**
