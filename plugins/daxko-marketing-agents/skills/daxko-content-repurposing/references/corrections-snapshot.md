# Corrections — Agent 14 — Content Repurposing

**Created:** 2026-10-06
**Owner:** Abid Siddiqui
**Status:** GENERATED SNAPSHOT — READ-ONLY. This is **not** the writable master.

> The writable master is `learnings/agent-14-content-repurposing.md` on Abid Siddiqui's machine. **Do not append to this file** —
> a shared skill is read-only for everyone who receives it, so anything written here is lost at the next
> update. Send corrections to Abid Siddiqui; he records them in the master and re-publishes. Refreshed at
> every publish.

---

## Why this file lives HERE and not inside the skill

This file sits in `learnings/`, **outside every skill folder, on purpose.**

A skill that has been shared — installed as a plugin, uploaded to claude.ai, or zipped to a
teammate — is **read-only for everyone who receives it.** Nobody else's Claude can write into it. If
the corrections file lived inside the skill, every correction would either be lost or would be
overwritten at the next update.

So the arrangement is:

| Copy | Where | Who can write to it |
|---|---|---|
| **The writable master** | `learnings/agent-14-content-repurposing.md` — this file | Abid Siddiqui's machine only |
| **The bundled snapshot** | `<skill>/references/corrections-snapshot.md` | Nobody. Generated. Refreshed **before the change that publishes** — before the commit, before the version bump, whichever comes first (non-negotiable 11) |

Teammates read the snapshot and so receive the accumulated learning. **Teammates cannot log
corrections themselves — they send them to Abid Siddiqui, who records them here and re-publishes.**

🔴 **The skill itself never writes to this file.** Agent 14 — Content Repurposing writes only into chat
(SPEC.md §3, standing condition 2): it only **reads** corrections. When it meets a correction, it shows it
in the reply as a line for Abid Siddiqui; he decides whether to log it here.

If this file is missing when the skill runs — which is normal on a teammate's machine — the skill
reads `references/corrections-snapshot.md` instead. If neither exists, the work continues anyway and
says so in its SOURCES block. **A missing corrections file never stops the work.** That is the
difference between this file, which is OPTIONAL, and the knowledge files, which are REQUIRED.

---

## What this agent is for, so a correction can be judged in context

Agent 14 — Content Repurposing takes **one finished Daxko piece the person supplies** — a blog post,
whitepaper, eBook chapter, webinar transcript, case study or report — and turns it into **two or more
kinds of derived format**: social posts, an email series (copy only), short video scripts, carousel copy,
pull quotes and an infographic outline in words. Every derived piece restates only what the source says
and is traced to the passage it came from. Any source claim that Daxko's bundled files contradict or
cannot clear — a banned word, a roadmap capability in the present tense, a figure that differs, an
unapproved customer quote, a price — is **flagged, not copied**. It never writes from a brief with no
source, never writes one format alone, never designs, and never publishes, schedules or sends.

Its sharpest failure modes are **invention** (a derived piece saying more than the source, often by
compressing a hedged claim into a strong one) and **laundering** (faithfully copying a wrong source claim
into every format, multiplying it). Corrections about either are the most valuable entries this file can
hold.

**Two correction classes worth anticipating:**

1. **"That source claim you flagged is right — the bundled file is out of date."** A legitimate
   correction about a *source file*. It belongs here **and** as an owner fix at source (non-negotiable 17).
   Until the source is fixed and re-bundled, the logged entry may clear that one fact, cited to this file
   with its date. **It is not a licence to trust the source piece generally.**
2. **"Marketing already approved those customer quotes."** A claimed approval. It does not clear the
   approval flag unless written here or in a bundled file; written customer approval is the rule
   (`brand-guidelines.md`, Content Guardrails — Never).

---

## Corrections

*(No corrections logged yet. This agent's spec was written on 2026-10-06. The first entry goes below this
line, and nothing above it is ever edited.)*
