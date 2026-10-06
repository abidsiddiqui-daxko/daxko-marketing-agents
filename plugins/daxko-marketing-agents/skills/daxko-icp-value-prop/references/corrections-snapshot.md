# Corrections — Agent 5 — ICP & Value Prop

**Created:** 2026-10-06
**Owner:** Abid Siddiqui
**Status:** GENERATED SNAPSHOT — READ-ONLY. This is **not** the writable master.

> The writable master is `learnings/agent-05-icp-value-prop.md` on Abid Siddiqui's machine.
> **Do not append to this file** — a shared skill is read-only for everyone who receives it, so
> anything written here is lost at the next update. Send corrections to Abid Siddiqui; he records
> them in the master and re-publishes. Refreshed at every publish.

---

## Why the writable master lives outside the skill

The writable master sits in `learnings/`, **outside every skill folder, on purpose.**

A skill that has been shared — installed as a plugin, uploaded to claude.ai, or zipped to a
teammate — is **read-only for everyone who receives it.** Nobody else's Claude can write into it. If
the corrections file lived inside the skill, every correction would either be lost or would be
overwritten at the next update.

So the arrangement is:

| Copy | Where | Who can write to it |
|---|---|---|
| **The writable master** | `learnings/agent-05-icp-value-prop.md` | Abid Siddiqui's machine only |
| **The bundled snapshot** | `references/corrections-snapshot.md` — this file | Nobody. Generated. Refreshed **before the change that publishes** — before the commit, before the version bump, whichever comes first (non-negotiable 11) |

Teammates read the snapshot and so receive the accumulated learning. **Teammates cannot log
corrections themselves — they send them to Abid Siddiqui, who records them in the master and re-publishes.**

🔴 **The skill itself never writes to either corrections file.** Agent 5 — ICP & Value Prop is read-only by owner
decision (D-2, 2026-10-06): it only **reads** corrections. When it meets a correction, it drafts a change
note in chat; Abid Siddiqui decides whether to log it in the master.

If the master is missing when the skill runs — which is normal on any machine but the owner's — the
skill reads this file instead. If neither exists, the work continues anyway and
says so in its SOURCES block. **A missing corrections file never stops the work.** That is the
difference between the corrections files, which are OPTIONAL, and the knowledge files, which are REQUIRED.

---

## What this agent is for, so a correction can be judged in context

Agent 5 — ICP & Value Prop is **Daxko's read-only reference for who we sell to and what we say to them.**
For a named market, segment, product or buyer role it answers from Daxko's approved files only: the
ideal customer profile, buying committee, pains, triggers, approved value proposition, proof points,
the Key Result the segment serves and what never to say — every line cited by file and line, every gap
marked `not in the files`, every contradiction between two files shown as a "files disagree" row with no
side picked. It can suggest one new value-proposition angle, always labelled **RECOMMENDATION — NOT
APPROVED POSITIONING**, and it can check a pasted brief against the documented buyers and approved
messages. It never edits a file, never writes a positioning document, never builds personas from
research and never writes copy.

Its sharpest failure mode is **inventing a person.** A profile agent that lacks a fact invents a persona,
a pain, a number, a quote, a capability or an approval — and because its answers feed other agents, the
invention is copied into every brief, deck and email downstream as if Daxko had approved it. Corrections
about any of those are the most valuable entries the corrections file can hold.

**Three correction classes worth anticipating:**

1. **"That persona / pain / approver is in a file you don't have."** A legitimate correction about a
   *source file*. It belongs in the master **and** as an owner fix at source — usually `knowledge-base/master-icps.md`
   (non-negotiable 17). Until the source is fixed and re-bundled, the logged entry may be used for that one
   fact, cited to the corrections file with its date. **It is not a licence to infer any other persona.**
2. **"Constance approved this Club positioning."** A claimed approval outside the scope the files give
   (Constance Miller is named for Nonprofit only). It does not bind the agent. If Abid Siddiqui confirms a
   Club or Boutique approver, it is written at source into `master-icps.md`, never only in the corrections file.
3. **"Pick the master-icps version — the playbook is out of date."** A ruling on one of the "files
   disagree" conflicts. The fix is at source in the losing file; until it is re-bundled, the agent keeps
   showing both versions. The corrections file records the ruling; it does not resolve the conflict in the skill.

---

## Corrections

*(No corrections logged yet. This agent was built on 2026-10-06.)*
