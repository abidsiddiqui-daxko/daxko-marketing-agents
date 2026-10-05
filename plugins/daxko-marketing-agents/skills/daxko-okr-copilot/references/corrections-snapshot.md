# Corrections — Agent 2 — OKR Copilot

**Created:** 2026-10-05
**Owner:** Abid Siddiqui
**Status:** GENERATED SNAPSHOT — READ-ONLY. This is **not** the writable master.

> The writable master is `learnings/agent-02-okr-copilot.md` on Abid Siddiqui's machine.
> **Do not append to this file** — a shared skill is read-only for everyone who receives it, so
> anything written here is lost at the next update. Send corrections to Abid Siddiqui; he records
> them in the master and re-publishes. Refreshed at every publish.

---

## Why this file lives HERE and not inside the skill

The writable master sits in `learnings/`, **outside every skill folder, on purpose.**

A skill that has been shared — installed as a plugin, uploaded to claude.ai, or zipped to a
teammate — is **read-only for everyone who receives it.** Nobody else's Claude can write into it. If
the corrections file lived inside the skill, every correction would either be lost or would be
overwritten at the next update.

So the arrangement is:

| Copy | Where | Who can write to it |
|---|---|---|
| **The writable master** | `learnings/agent-02-okr-copilot.md` | Abid Siddiqui's machine only |
| **The bundled snapshot** | `references/corrections-snapshot.md` — this file | Nobody. Generated. Refreshed **before the change that publishes** — before the commit, before the version bump, whichever comes first (non-negotiable 11) |

Teammates read this snapshot and so receive the accumulated learning. **Teammates cannot log
corrections themselves — they send them to Abid Siddiqui, who records them in the master and
re-publishes.**

If the master is missing when the skill runs — which is normal on any machine but the owner's — the
skill reads this file instead. If neither exists, the work continues anyway and says so in its
SOURCES block. **A missing corrections file never stops the work.** That is the difference between
this file, which is OPTIONAL, and the knowledge files, which are REQUIRED.

---

## What this agent is for, so a correction can be judged in context

Agent 2 — OKR Copilot is **the planner of what Daxko will do against its objectives.** It turns
Daxko's OKRs — a company, market or team objective, or a named Key Result — into a draft plan for a
quarter: what to do, in what order, the **role** that owns each piece, proposed timing, and which Key
Result each item serves. It also re-plans after a Key Result is reported behind (from Agent 18 —
Marketing Performance's reading or the person's own premise), and checks an existing plan for work
that serves no Key Result. It plans **in chat only**: it reads no numbers into a status, fetches
nothing, and writes into no system — no Asana task, no Airtable record, no file.

Its sharpest failure mode is **inventing a commitment.** A writer's invention is a sentence a reader
can fact-check; a planner's invention is a promise with a name and a date on it — a quarter's target
nobody set, an expected result nobody estimated, a named owner nobody agreed, a budget nobody
approved, a product scheduled into a quarter it does not ship in. Inside a plan, each reads as
already agreed. Corrections about any of those — and about a status word given in the agent's own
voice — are the most valuable entries this file can hold.

**Three correction classes worth anticipating:**

1. **"That placeholder is a known figure — the Q4 slice is in the targets spreadsheet."** A
   legitimate correction about a *source file*. It belongs in the master **and** as an owner fix at
   source, where quarterly targets belong (`okrs-and-priorities.md` or `performance-data-schema.md`)
   — non-negotiable 17. Until the source is fixed, the logged entry may be used for that one figure,
   cited to the corrections file with its date. **It is not a licence to slice any other target.**
2. **"We use 80% of pace as on track."** A claimed rule not in the knowledge files does not bind the
   agent. If Abid Siddiqui adopts it, it is written at source into `performance-data-schema.md` and
   applied by Agent 18 — Marketing Performance — **never by this agent** (assumed owner answer Q1).
3. **"Put Jane on the webinar item."** A person-supplied owner for **one** plan — used as given in
   that plan. It is never logged as a standing rule to assign future work to a named person.

---

## Corrections

*(No corrections logged yet. This agent was built on 2026-10-05.)*
