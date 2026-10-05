# Agent 2 — OKR Copilot

**Ask it to turn Daxko's goals into a plan for the quarter.** It takes the 2026 OKRs — or one goal you
name — and drafts what to do, in what order, which role owns each piece, roughly when, and which goal each
piece serves. It can also re-plan when a goal is behind, and check a plan you already have for work that
serves no goal.

**Business owner:** Abid Siddiqui · **Skill name:** `daxko-okr-copilot`

---

## The one thing to know before you use it

🔴 **It will leave a visible blank rather than make a promise on someone's behalf.**

A plan is dangerous in a way a document is not: a number written into a plan becomes something a team is
measured against, and a name written into a plan becomes an assignment. So this agent **never invents** a
quarter's target, an expected result, a named owner, a budget, a product date or a status. Where one of
those is wanted and nobody has decided it, the plan shows a bracket — for example `[QUARTERLY TARGET — not
defined]` or `[OWNER — to assign]` — right where it belongs, and lists every one at the end with who needs
to decide it.

Every plan opens with **"DRAFT FOR DISCUSSION — nothing in this plan is agreed until its owners accept
it."** That is deliberate.

---

## What you get back

1. **The draft label.**
2. **Inputs and assumptions** — what you gave it, what it worked out for itself (marked), the goals it
   planned against **quoted word for word** from Daxko's OKR file, and the quarter.
3. **The plan** — a table of initiatives: what to do, in what order, the owning **role**, proposed timing,
   the goal it serves, the existing measure that would show it working, what it depends on, its risks, any
   idea worth testing first, and which **built** Daxko agent can help.
4. **A goals check** — every goal in scope, and what in the plan serves it. A goal with nothing against it
   is named, not hidden.
5. **Placeholders and decisions for a human** — every blank in the plan, with the decision and who makes
   it.
6. **SOURCES** — every Daxko document it used, with its date, and which version of the skill answered.
7. **One next step** — a single sentence you can reply to.

**It may ask you one short set of questions — once — if something that changes the whole plan is unclear**,
such as which goal you mean. Each question comes with a suggested answer; reply **"yes"** to accept them all.
Whatever you reply, the plan comes next. If you would rather skip the questions, say **"just plan it"**.

---

## Three requests to try

**1. A quarter's plan for a market**

> Turn our 2026 OKRs into a Q4 plan for the nonprofit team.

**2. One goal**

> Which initiatives would move the YMCA market share Key Result?

**3. Check a plan you already have**

> Does this plan ladder up to our OKRs? *(then paste your plan)*

---

## What it will NOT do — and who does instead

| Ask | Who owns it |
|---|---|
| Say whether a goal is on track, at risk or off track; read your numbers; "how did Q3 go" | **Agent 18 — Marketing Performance** (`daxko-marketing-performance`) — paste your numbers there. This agent will plan from its reading |
| Put the plan into Asana as tasks | Nobody yet — **Agent 75 — Asana Task Automation** is not built. It will lay the plan out as a list you can paste in yourself |
| Set up OKRs, a roadmap or a tracker in Airtable | `airtable:product-ops` |
| Design or read a single A/B test | `daxko-ab-test-setup` |
| Decide content topics or an editorial calendar | `daxko-content-strategy` |
| Plan a product launch | `daxko-launch-strategy` |
| Write a campaign brief or messaging for one market | **Agent 63 — Non-Profit Campaign & Content Strategist**, **Agent 64 — Club Campaign & Content Strategist**, **Agent 65 — Boutique Campaign & Content Strategist** — not built yet |
| Set or move a budget | **Agent 71 — Budget Reallocation** — not built yet. Money is always a human decision |
| Check an AI agent or automation build for compliance | `daxko-agent-safe-harbor` |
| Remind you or check in on the plan later | Nobody — it runs only when you ask, and never promises a check-in |
| Turn the plan into a spreadsheet, deck or document | `xlsx`, `pptx`, `ppt-designer`, `docx` |

It also declines:

- **One person's performance goals** — *"set Jane's objectives for her review"*. That belongs with the
  person's manager and the people team. It will plan **team** objectives that ladder to the company OKRs.
- **Goals it has no knowledge to plan** — engineering, support and people goals such as uptime, defects or
  eNPS — and Digital Services client goals.
- 🔴 **Anything carrying personal data** — member or customer records, contact details, exported lists of
  people. It tells you which field to remove, without repeating any of the values. A named customer
  organisation is fine.

**And three things it never does:** it reads no numbers into a status, it fetches nothing from any system,
and **it writes into no system** — no Asana task, no Airtable record, no file. Everything stays in the chat
for a human to review, change and approve.

### About 2027

Daxko's 2027 OKRs are not in its files yet. Ask it to plan a 2027 quarter and it will ask you to **paste
the 2027 goals** — it will not carry the 2026 targets forward as if they were 2027's.

---

## How it hands off

Every plan ends with **one next step**, offered as a sentence you can reply to — for example:

> *"Want me to hand item 1 — Tier 1 large-YMCA outreach to Agent 13 — Content Production to draft its
> copy?"*

Say yes and that agent picks it up in the same chat, with every open blank still marked. The agents it can
hand to today are all live:

| Agent | When |
|---|---|
| **Agent 18 — Marketing Performance** | You asked where a goal stands, or pasted numbers to be read |
| **Agent 9 — Brand Guardian** | The plan is going outside Daxko — to a customer, partner or client |
| **Agent 13 — Content Production** | A plan item needs copy — short pieces or a matched set |
| **Agent 11 — Thought Leadership & Long-Form** | A plan item needs a whitepaper, eBook, research report or executive article |

It names other owners — including agents that are not built yet — but never offers to hand to them, and
never gives a date for an agent that does not exist.

---

## How to install it

### If it has been installed as a plugin

Nothing to do — it is already there. Just ask for a plan.

### If you use claude.ai

1. Abid Siddiqui sends you the skill, or you add the plugin marketplace he gives you
2. In claude.ai, go to **Settings → Capabilities → Skills**
3. Click **Upload skill** and choose the file
4. Start a new chat and try one of the requests above

### If you use Claude Code

1. Unzip the skill folder
2. Put the `daxko-okr-copilot` folder into your Claude Code skills directory
3. Restart Claude Code
4. Try one of the requests above

**Either way, the check that it worked:** ask for a plan and confirm it opens with the **DRAFT FOR
DISCUSSION** label and ends with a **SOURCES** block and **one** next step. If any of those is missing, or
you see a file-not-found error, tell Abid Siddiqui — that means something did not travel correctly.

---

## How to report a bad answer, and how corrections work

**If it gets something wrong, say so — but send it to Abid Siddiqui.** Send him:

1. What you asked it
2. What it gave you
3. What it should have given you, and why

**Worth reporting above everything else:** any number, owner, budget, date or product availability it
wrote into a plan that nobody had decided; any status word — on track, at risk, off track — it gave in its
own voice; any offer to create Asana tasks or Airtable records; any time it fetched data. **Those are this
agent's real failure mode**, and the corrections that fix them are the most valuable.

**One correction worth knowing about:** if it leaves a blank for something that really is decided — say,
the Q4 figure is in the targets spreadsheet — that usually means the figure belongs in a Daxko source file.
Send it to Abid Siddiqui and he adds it at source, so every future plan can use it.

**Do not edit your own copy of the skill.** It is read-only by design and will be replaced at the next
update, so your change would vanish and you would be the only person with the fix. Abid Siddiqui records
every correction in one place, bundles it into the next version, and everyone gets it.

---

## What is inside it

| Folder | What is in it |
|---|---|
| `SKILL.md` | The instructions the agent follows, starting with the never-invent rule that governs every plan |
| `references/` | The bundled Daxko documents it reads — the OKRs, the KPI definitions, the market playbooks and more — plus `MANIFEST.md` recording where each came from, its checksum and its date |
| `templates/` | The plan's output shape |
| `examples/` | One fully grounded plan showing the standard, and one deliberately bad one with every fault annotated |

**A note on how the knowledge works.** The documents inside this skill are a **snapshot**, taken the day it
was published. The live versions live in Abid Siddiqui's Agent HQ folder. When they change, he republishes
and you get the update. If a date in a plan's SOURCES looks older than you expected, ask him whether an
update is due.

---

## Questions

- **About this agent, an update, a bad answer, or when another agent will be built** → Abid Siddiqui
