# Agent 11 — Thought Leadership & Long-Form

**Ask it to write one long, authoritative piece.** It drafts a single whitepaper, eBook manuscript, industry
or research report, or executive byline article that positions Daxko as an authority — grounded entirely in
bundled Daxko knowledge, with every unsourced fact left as a visible placeholder instead of a guess.

**Business owner:** Abid Siddiqui · **Skill name:** `daxko-thought-leadership`

---

## The one thing to know before you use it

🔴 **It would rather leave an obvious blank than write a convincing lie.**

A whitepaper is the format where a made-up statistic does the most damage, because under a chart and an
executive's byline it looks like evidence. So this agent never invents a statistic, a customer, a quote, a
price, a date or a product capability. Where a real fact is wanted and no bundled Daxko file supports it, it
writes a visible `[PLACEHOLDER]` in the text and lists it at the end — so you know exactly what to source
before the piece can publish.

It also writes a roadmap capability as *coming*, never as *shipped* — the difference between a tool you can
sell today and a promise you cannot.

---

## What you get back

It works in two steps, and the first one is quick:

1. **It locks the thesis and outline first**, and offers them to you — *"here is the thesis and outline; want
   me to draft the full manuscript, or adjust the outline first?"* If you would rather it just wrote the whole
   thing, say **"just write it"** and it drafts the full piece in one pass, marking any assumptions it had to
   make. It asks once and never holds your draft hostage.
2. **Then it drafts the manuscript** — the full piece, section by section, ready to paste — followed by a
   **SOURCES** list, a **placeholders-and-gaps** list of every fact you still need to supply, the **Key
   Result** the piece maps to, and **one next step**.

---

## Three requests to try

**1. A whitepaper**

> Draft a short whitepaper for YMCA and JCC executives on how AI is changing member engagement, positioning
> Daxko as the authority.

**2. A research / state-of-the-industry report**

> Author a state-of-the-industry report on payments and member retention for boutique studio owners.

**3. An executive byline article**

> Ghostwrite a point-of-view article our VP can put her name to, on why fitness clubs should treat AI as a
> member-relationship tool, not a marketing gadget.

---

## What it will NOT do

| Ask | Who owns it |
|---|---|
| A **set** of short assets from one message — social, email, ads, landing page | **Agent 13 — Content Production** (`daxko-content-production`) |
| Plan, gate or distribute a lead magnet — an email-capture offer, or what to give away for emails | `daxko-lead-magnets` |
| A search-optimized blog post or article | **Agent 12 — Blog & Article** / `daxko-ai-seo` |
| Slice one finished piece into many derived formats | **Agent 14 — Content Repurposing** |
| Decide what to write about — topics, gaps, the editorial calendar | **Agent 10 — Content Strategy** / `daxko-content-strategy` |
| Copy for one named product brand or vertical audience | `daxko-nonprofit-copywriter`, `club-automation-copywriter`, `zen-planner-copywriter` |
| Judge whether the draft is on brand, or approve it to publish | **Agent 9 — Brand Guardian** |
| Design, lay out or format the finished file | **Agent 29 — UX/UI Design**, and `docx` / `pdf` / `pptx` / `ppt-designer` |

It will write an **art-direction note in words** — "cover: a studio owner reviewing a report at the front
desk" — but no colour, no font and no layout; those belong to the designer.

It also declines non-marketing material — code, legal or contract text, HR documents — and 🔴 **stops if your
request carries personal data** — member names, contact details, dates of birth, payment or health data. It
tells you which category to remove, without repeating the values, and writes the piece once the data is out. A
named customer organisation or an approved case-study customer is fine — that is marketing content, not
personal data.

**It publishes nothing.** It writes a draft in chat for a human to review, edit and publish. It does not
schedule, send, gate or design anything.

---

## How it hands off

Every manuscript ends with **one next step**, offered as a sentence you can reply to. The default, on every
piece, is a brand check:

> *"Want me to send this to Agent 9 — Brand Guardian for a brand check before you publish?"*

Say yes and Agent 9 — Brand Guardian picks the manuscript up in the same chat. A long-form authority piece is
external content, and every external piece gets a brand check before it goes out. From there it can also go to
**Agent 13 — Content Production** to be spun into a launch set, to **Agent 29 — UX/UI Design** to be designed,
or to **Agent 10 — Content Strategy** to decide what to write next.

---

## How to install it

### If it has been installed as a plugin

Nothing to do — it is already there. Just ask it to write a piece.

### If you use claude.ai

1. Abid Siddiqui sends you the skill, or you add the plugin marketplace he gives you
2. In claude.ai, go to **Settings → Capabilities → Skills**
3. Click **Upload skill** and choose the file
4. Start a new chat and try one of the requests above

### If you use Claude Code

1. Unzip the skill folder
2. Put the `daxko-thought-leadership` folder into your Claude Code skills directory
3. Restart Claude Code
4. Try one of the requests above

**Either way, the check that it worked:** ask for a whitepaper and confirm you get back a **thesis and
outline** first, and — after the draft — a **SOURCES** block and a **placeholders-and-gaps** list. If any of
those is missing, or you see a file-not-found error, tell Abid Siddiqui — that means something did not travel
correctly and he needs to know.

---

## How to report a bad answer, and how corrections work

**If it gets something wrong, say so — but send it to Abid Siddiqui.** Send him:

1. What you asked it
2. What it gave you
3. What it should have given you, and why

**Worth reporting above everything else:** any invented statistic presented as fact, any customer or quote it
made up, any roadmap capability it described as already shipped, or any place it softened a made-up number
into a vague one instead of leaving a placeholder. **Those are this agent's real failure mode**, and the
corrections that fix them are the most valuable entries in the file.

**One correction worth knowing about:** if it leaves a `[PLACEHOLDER]` for a figure that actually is a known,
sourced number, that usually means the number belongs in a source file (`product-knowledge.md` or
`competitive-intel.md`). Send it to Abid Siddiqui — he adds it at source so every future piece can use it. It
is not a reason to let the agent start writing unsourced numbers.

**Do not edit your own copy of the skill.** It is read-only by design and will be replaced at the next update,
so your change would vanish and you would be the only person with the fix. Abid Siddiqui records every
correction in one place, bundles it into the next version, and everyone gets it.

---

## What is inside it

| Folder | What is in it |
|---|---|
| `SKILL.md` | The instructions the agent follows, including the no-invention rule that governs every piece |
| `references/` | The bundled Daxko documents it reads, plus `MANIFEST.md` recording where each came from, its checksum and its date |
| `templates/` | The manuscript output shape — lock the thesis, offer, then draft |
| `examples/` | One fully grounded whitepaper showing the standard, and one deliberately bad one with every fault annotated |

**A note on how the knowledge works.** The documents inside this skill are a **snapshot**, taken the day it
was published. The live versions live in Abid Siddiqui's Agent HQ folder. When they change, he republishes and
you get the update. Your copy is read-only by design — that is what keeps everyone writing from the same brand
rules and the same facts.

---

## Questions

- **About this agent, an update, or a bad answer** → Abid Siddiqui
- **About Daxko brand voice, before a piece goes out** → Anna Klement, Communications Manager
