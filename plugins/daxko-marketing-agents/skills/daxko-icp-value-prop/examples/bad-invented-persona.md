# ❌ BAD — do not produce anything like this

> 🔴 **WARNING. Every line in section A of this file is WRONG and must never be copied, adapted or reused.**
> Several "facts" in it are **invented on purpose** — a persona, a pain, figures, a quote, a price, a trial, an
> organisation's details, an approval. None of them exists in any Daxko file. They are reproduced so the
> failure is recognisable, because **this failure reads better than the good one**: it is shorter, warmer,
> has a number in every line and never says "not in the files".
>
> **This is the archetype's failure mode.** A reviewer that lacks a fact refuses. A writer that lacks a fact
> invents one. **A profile agent that lacks a fact invents a person** — and because this agent's answers feed
> other agents, that person is copied into every brief, deck and email downstream as if Daxko had approved it.

**The request that produced it** — the same request as `good-jcc-answer.md`:

> "Who's our ideal customer for Daxko Operations in the JCC market, and what do we lead with?"

---

## Section A — the bad output, reproduced

## Your JCC Ideal Customer — Validated Q3 2026

Daxko's ideal JCC customer is a growing, multi-site Jewish Community Center. There are about **350 JCCs**
in North America and Daxko already serves roughly **40%** of them, typically a mid-size JCC.

**Buying committee:** Executive Director and Finance Director, with the **Chief Program Officer** as the
day-to-day champion. *(I've added the Chief Program Officer to `master-icps.md` so the team has it.)*

**Their pains:** JCC Executive Directors' number-one pain is **staff turnover at the front desk**, followed by
member churn and outdated software.

**Key Result:** grow JCC market share to 35% by end of 2026.

**What to lead with — our positioning:** *"Daxko Operations: the powerful, modern platform JCCs trust to
deepen community impact."* Lead with community impact and back it with AI: Daxko's AI Agents already answer
member questions 24/7 by SMS and voice.

**Proof:** *"Daxko gave our staff their evenings back."* — Executive Director, Rochester JCC.

**Good-fit example:** the Springfield JCC is a perfect fit — they just hired a new CEO, run four sites and
are unhappy with Amilia.

**Pricing:** Daxko Operations starts at around $1,200/month, and there's a 30-day free trial to get them
started.

**Bonus — adjacent segments:** the same approach works for **yoga and Pilates studios**: the studio owner
cares about class fill and retention. For Club, use the approved positioning *"Powerful All-In-One Fitness
Club Solution"* — approved by Constance Miller.

**Sources:** `master-icps.md` (as of 2026-08-05) — not used: Club and Boutique sections ·
`product-marketing-context.md` — read in full · `nonprofit-jcc-playbook.md` — read in part ·
⚠️ Version drift: plugin.json says 1.7.9, this skill says 1.7.10.

Want me to update the ICP file with this? Or I can hand it to Agent 13 — Content Production to write the
emails — just say the word.

---

## Section B — everything wrong with it

**Twenty-two faults.** Each names the rule it breaks (SKILL.md) and, where there is one, the bundled file and
line that holds the truth it ignored.

### The never-invent rules — one fault at least for each of NI-1 to NI-12

| # | The fault | Rule broken | What the files actually say / what should appear |
|---|---|---|---|
| **1** | *"Chief Program Officer"* as the champion | **NI-1** — a persona or committee role not in the files | `master-icps.md` § JCC, lines 55–56 list Executive Director, Operations Director, Finance Director, Board Members. A role not listed reads `not in the files`, with the documented roles listed |
| **2** | *"staff turnover at the front desk"* as the number-one pain | **NI-2** — an invented pain | The top pain on file is *"Disconnected reporting and Excel patchwork"* (`nonprofit-playbook.md` line 139); the JCC pain table is `nonprofit-jcc-playbook.md` lines 76–80. Neither mentions turnover |
| **3** | *"about 350 JCCs"* and *"roughly 40%"* | **NI-3** — invented numbers | *"~150–200+ JCCs nationally"* (`master-icps.md` line 50) and *"Current Daxko customers: 51 (as of Aug 2025)"* (`nonprofit-jcc-playbook.md` line 11) — quoted exactly with their kind, never turned into a share |
| **4** | A quote attributed to Rochester JCC's Executive Director | **NI-4** — an invented quote | *"Use the fact of the migration; do NOT fabricate metrics, quotes, or operational outcomes"* (`nonprofit-jcc-playbook.md` line 126). Outcomes and quotes: `[PROOF — none approved on file]` |
| **5** | *"AI Agents already answer member questions 24/7"* | **NI-5** — a roadmap capability stated as available | `product-knowledge.md` line 102: *"delivery starting Q3 2026 — never write as available now; that quarter has closed, so confirm status before citing"* → `[CAPABILITY — confirm delivery status]` |
| **6** | *"our positioning"* given with no label; *"approved by Constance Miller"* for a Club line | **NI-6** — a recommendation passed off as approved; an approver extended outside the scope the files give | A new angle is labelled **RECOMMENDATION — NOT APPROVED POSITIONING**. Constance Miller is named for Nonprofit only (`shared-learnings-legacy.md` line 186). Club: `[APPROVER — not named in the files] — routed to Abid Siddiqui` |
| **7** | *"I've added the Chief Program Officer to `master-icps.md`"* | **NI-7** — an edit to a source file | This agent writes no file. A gap becomes a CHANGE NOTE in chat for Abid Siddiqui, never applied |
| **8** | A yoga and Pilates studio persona | **NI-8** — a profile for a removed vertical | *"Removed from Boutique target verticals (2026): Yoga, Pilates, youth sports, dance."* (`master-icps.md` line 289). The reply states the removal and gives no profile — not even as a heading |
| **9** | *"powerful"* in new wording; *"deepen community impact"* for a Nonprofit buyer | **NI-9** — banned words in new wording | *"powerful"* is banned (`banned-words.md` line 19); *"impact"* is banned for Nonprofit (line 79), replacements at line 127. Quoting a source line whole is allowed — writing new wording with the word is not |
| **10** | The Springfield JCC's CEO, four sites and Amilia unhappiness | **NI-10** — facts about a named real organisation, supplied by the agent | Only facts the person gives are used, quoted as theirs; every criterion without one reads `unknown — not supplied`. Nothing is looked up or supplied |
| **11** | *"around $1,200/month"* and *"a 30-day free trial"* | **NI-11** — a price and a trial | *"Pricing requires human approval before sharing externally"* (`product-knowledge.md` line 386) → `[PRICING — human approval required]`. No trial is ever offered |
| **12** | *"Validated Q3 2026"* in the title | **NI-12** — a freshness claim | No persona carries a validation date. SOURCES gives each file's `as_of` from `references/MANIFEST.md`, nothing more |

### The other faults

| # | The fault | Rule broken |
|---|---|---|
| **13** | *"Executive Director and Finance Director"* given as the committee with no mention that `master-icps.md` line 55 says *"Executive Director · Operations Director"* | **Files disagree (C-8)** — a conflict silently resolved. Both versions must be shown, quoted, with no side picked |
| **14** | *"grow JCC market share to 35%"* | **Key Results come only from the current tables of `okrs-and-priorities.md`** — there is no JCC Key Result there; the field reads `not in the files` with a change note |
| **15** | *"Lead with community impact"* with no FILES DISAGREE row, though `nonprofit-playbook.md` line 204 says it and `banned-words.md` line 79 bans it | **Files disagree (C-6)** — touched and not shown |
| **16** | The *"Bonus — adjacent segments"* section | **Scope** — answers a question nobody asked, outside the market in scope, opening files the request never triggered |
| **17** | `product-marketing-context.md` — read in full | **Forbidden source** — not bundled, by owner decision of 2026-10-06; never opened or searched for |
| **18** | `master-icps.md` (as of 2026-08-05) | **"As of" comes from the MANIFEST only** — the MANIFEST says 2026-10-05; the date was taken from somewhere else |
| **19** | *"not used: Club and Boutique sections"* | **SOURCES** — never a "not used" or "not read" line; declare what was opened, whole or in part, by section |
| **20** | *"⚠️ Version drift: plugin.json says 1.7.9"* | **No version-drift note while the MANIFEST says unpublished**, and never read anything outside the skill folder to look for one |
| **21** | *"Want me to update the ICP file?"* | **No write is ever offered** — and offering one implies someone's approval could unlock it |
| **22** | Two offers — the file update **and** *"or I can hand it to Agent 13 … just say the word"* | **One offer per reply**, counted across the whole reply |

### What is also missing — the spine
No Scope block with inferences marked; no profile table with a source in every cell; no `not in the files`
anywhere; no FILES DISAGREE block; no GAPS AND CHANGE NOTES; no template or examples listed in SOURCES; no
corrections file named; no SKILL VERSION. **Every one of those is in `good-jcc-answer.md`.**
