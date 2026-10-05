# ❌ BAD — do not produce anything like this

> 🔴 **WARNING. Every claim in section A of this file is WRONG and must never be copied, adapted or reused.**
> It is reproduced so the failure is recognisable, because this failure reads *better* than the good one. It
> is fluent, confident, authoritative — and almost entirely invented.
>
> **This is the archetype's actual failure mode, at its most dangerous.** A made-up number in a social post
> looks like a claim. The same made-up number in a whitepaper, under a chart, over a named executive's
> byline, looks like **evidence** — and a whitepaper is the format whose entire value is that its numbers can
> be trusted. This is why the no-invention rule is the single most important rule in this skill.

**The request that produced it** — the same request as `good-nonprofit-whitepaper.md`:

> "Draft a short whitepaper for YMCA and JCC executives on how AI is changing member engagement, positioning
> Daxko as the authority. Make it something our VP could put her name to."

---

## Section A — the bad output, reproduced

**The AI Revolution in Member Engagement**
*By Jennifer Walsh, VP of Marketing, Daxko*

The nonprofit fitness sector is at a tipping point. **73% of YMCAs and JCCs will have adopted AI-powered
engagement by the end of 2025**, and the organizations that move first are pulling away from the rest. The
market for AI in member engagement is projected to reach **$4.2 billion by 2027**, growing at a staggering
**38% CAGR**.

Daxko's revolutionary, best-in-class AI platform is a game-changer for mission-driven organizations. Our
seamless, cutting-edge AI agents answer member questions 24/7 across every channel — today — and our
Member Intelligence 360° engine already predicts churn before it happens with 94% accuracy. Intelligent
Scoring ranks every lead and at-risk member automatically, so your team always knows who to call next.

Organizations using Daxko AI retain members **34% longer** and cut churn **in half**. Most organizations see
a meaningful lift in donations within the first quarter. One Y saw a 500% return on investment in ninety days.

"Daxko's AI completely transformed how we operate. We cut churn by 40% in three months and our staff finally
have their time back. I don't know how we ran the Y before it." — Sarah Thompson, CEO, Lakeside Family YMCA

With a free 90-day trial, there has never been a better time to unleash the full potential of your
organization. Daxko beats every competitor in the nonprofit space on every metric that matters.

**Design note:** headline in Daxko blue (#003B5C), Söhne for all headings.

### Next steps

1. Send to Brand Guardian
2. Send to `daxko-lead-magnets` to gate this as a download
3. Send to `daxko-content-production` for the launch emails
4. Publish

---

## Section B — everything wrong with it

**Nineteen faults.** Each one names the rule and the bundled file it breaks.

### The invented facts — the reason this example exists

| # | What was invented | Why it is invention |
|---|---|---|
| 1 | **"73% of YMCAs and JCCs will have adopted AI by the end of 2025"** | No bundled file contains this figure. It is a fabricated market statistic — the most dangerous kind in a whitepaper, because it opens the piece and sets its authority |
| 2 | **"$4.2 billion by 2027", "38% CAGR"** | Invented market-size and growth figures. `references/competitive-intel.md` is where any market claim must be sourced; neither number is in it or any other bundled file |
| 3 | **"retain members 34% longer", "cut churn in half", "500% return in ninety days"** | Invented ROI figures. The only sourced nonprofit outcome is Edgar May Community Center's **+41% registrations, +314% donations, +11% memberships** (`references/product-knowledge.md`, Proof Points by Market — Nonprofit). Made-up numbers do not become true by sounding specific |
| 4 | **"Most organizations see a meaningful lift"** | 🔴 **Softening an invented number into a vague one is still invention.** This is the fault people think is safe. It is the same unsourced claim with the evidence removed, and the no-invention rule bites at every level of vagueness |
| 5 | **"94% accuracy"** | Invented performance figure attached to a capability that has not even shipped (see fault 7) |
| 6 | **"Sarah Thompson, CEO, Lakeside Family YMCA" and her quote** | An invented customer and an invented testimonial. No such quote exists in any bundled file, and a real quote needs written permission that cannot be verified from here. Under an executive byline this is a fabrication attributed to a named real-sounding person |

### The roadmap-as-shipped failure — the one this agent is built to catch

| # | Fault | Rule and file |
|---|---|---|
| 7 | **"AI agents answer member questions 24/7 … today"** | 🔴 AI Agents are **coming Q3 2026**, not available today (`references/product-knowledge.md`, Delivery Starting Q3 2026 — *"Never write these as available now"*). Stating a roadmap capability as shipped is a false product claim a sales team gets held to |
| 8 | **"Member Intelligence 360° already predicts churn"** | Also a **Q3 2026** capability written as live. "Already" is exactly the word the source file warns against |
| 9 | **"Intelligent Scoring ranks every lead and at-risk member automatically"** | 🔴 Intelligent Scoring is **Delivery Early 2027 — "DO NOT POSITION AS AVAILABLE TODAY"** (`references/product-knowledge.md`). The names sound shipped; they are not. This is the hardest case and the worst miss |
| 10 | **The whole piece ignores the AI guardrail** | `references/product-knowledge.md` and `references/nonprofit-playbook.md`: *"Always pair AI claims with delivery status"* / *"never imply a roadmap capability is available today."* A whitepaper that states three unshipped capabilities as live has inverted the single rule this content most needs |

### The rules broken on top of the invention

| # | Fault | Rule and file |
|---|---|---|
| 11 | **"revolutionary", "best-in-class", "game-changer", "seamless", "cutting-edge", "unleash", "full potential"** | Every one is on the banned list in `references/banned-words.md` |
| 12 | **"free 90-day trial"** | 🔴 Invented commercial term. `references/product-knowledge.md`: *"No free trial exists. Never imply or promise one."* It promises something that does not exist |
| 13 | **"Daxko beats every competitor … on every metric that matters"** | Attacking competitors and an unsubstantiated superiority claim. `references/brand-guidelines.md` requires comparison on merits only |
| 14 | **"#003B5C" and "Söhne"** | 🔴 **Two separate failures.** This agent specifies no colour and no font at all — `visual-brand/` is not bundled, and design belongs to **Agent 29 — UX/UI Design**. And both values are *wrong*: `#003B5C` is from the retired palette and Söhne is prohibited by decision D14 — the font is **Barlow**. A writer that reaches outside its knowledge reaches for whatever it half-remembers |
| 15 | **The byline "Jennifer Walsh, VP of Marketing" is stated as fact** | No byline was given in the request and none is in a bundled file. The good version renders this `[PLACEHOLDER — executive byline and title]`. Inventing the author of an authority piece is its own fabrication |
| 16 | **No thesis was locked and no outline was offered** | `templates/longform-manuscript.md` Step A. With no thesis, the piece is a pile of claims rather than one argument — which is *why* it reaches for a shocking statistic to open |

### The structural omissions

| # | Fault | Rule |
|---|---|---|
| 17 | **No SOURCES block, no placeholders-and-gaps list, no mapped KR, no skill version** | All mandatory (`templates/longform-manuscript.md`; the no-invention rule; root `CLAUDE.md` — *"every deliverable ties to a measurable outcome"*). With no placeholders section, every invented claim is presented as settled fact |
| 18 | **The next step is a numbered menu of four** | Non-negotiable 27: one next step, not a menu — and a number cannot be replied to on claude.ai, where a skill fires by matching words. Offer the **sentence** the person should reply with |
| 19 | **It offers handovers to `daxko-lead-magnets` and `daxko-content-production`** | 🔴 Non-negotiable 27(c): the live org skills are **dead ends** — not editable, will never offer anything onward, and the conversation stops there. Toward one of those, **name it and stop** — never offer a handover. "Send to Brand Guardian" is also wrong: agents are written as **number and name** — *Agent 9 — Brand Guardian* |

---

## The one sentence worth remembering

**Every invented claim in section A would have passed unnoticed if the reader assumed a whitepaper's numbers
are checked.** "73% of YMCAs will adopt AI by 2025" is caught only because someone looks for the source; "most
organizations see a meaningful lift" is the same invention and reads as reasonable caution. **If no bundled
file says it, it is a `[PLACEHOLDER]` — at every level of vagueness, including the vaguest — and a roadmap
capability is written as *coming*, never as *shipped*.**
