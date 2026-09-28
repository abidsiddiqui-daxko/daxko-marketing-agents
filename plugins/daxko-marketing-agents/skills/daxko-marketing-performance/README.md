# Agent 18 — Marketing Performance

**Paste your numbers into the chat, then ask what they mean.** It reads marketing figures that are
already in the conversation and tells you how a period went against a Daxko Key Result — for Daxko's
own marketing and for Digital Services' client work.

**Business owner:** Abid Siddiqui · **Skill name:** `daxko-marketing-performance`

---

## The one thing to know before you use it

🔴 **It does not go and get your data. You bring the data; it brings the meaning.**

Pull your numbers into your Claude chat first — run your GA4 connector, paste a spreadsheet, drop in
an export — **and then ask the question.** If you ask before pasting anything, it will tell you
exactly what to paste rather than guessing or making something up.

That is a deliberate design choice, not a limitation we are working around. It means the answer never
depends on whether a connector is healthy that morning — and two of Daxko's are not: **Salesforce is
connected for nobody**, and Google Search Console is currently dead on all five properties.

---

## What you get back

The length changes to fit your question — a one-line question gets a short answer, not a report. But
five things are in **every** answer, at every length:

1. **Coverage** — what data it got and, by name, **what it did not get.** This comes first, before any
   finding. If you sent four of six sites, it says so and will not talk about "the portfolio".
2. **The answer**, sized to the question.
3. **Every number labelled and dated** — whether each figure is a target or a real result, and when it
   was actually measured.
4. **A sources list** that declares its own limits — every Daxko document it opened with its date,
   which ones it read only in part, and which version of the skill answered.
5. **One next step** — a single sentence, usually a brand check with Agent 9 — Brand Guardian, or
   campaign copy from Agent 13 — Content Production.

**It will ask you up to five short questions — once, in one message, with a default for each.** Reply
*"yes"* and it runs with all the defaults. It works out whatever it can from your data instead of
asking (period, market, own-versus-client) and tells you what it assumed. **If you ignore the
questions and say "just do it", it produces the report against the defaults and marks every
assumption.** It will never hold your answer hostage to a reply.

---

## Three requests to try

**1. The whole quarter**

> How did Q3 go for nonprofit? Here are the GA4 numbers and the pipeline export.

**2. One goal, one status**

> Are we on track for the nonprofit pipeline KR? Pipeline figures below.

**3. One thing**

> Did that email campaign work? Sends, opens, clicks and the demo requests it produced are pasted
> below.

---

## The four things it refuses to do, and why they matter

These are the reasons to trust it, so they are worth reading rather than skipping.

**1. It will not make a whole number out of a partial one.** Send four of six brands and ask how the
portfolio did, and you get *"up across the four brands you provided — named; these two were not
provided."* Never *"up across the portfolio"*. The gap is always named.

**2. It will not report old numbers as current.** Every figure carries the date it was **measured**,
not the date the file was written. Daxko's objectives file currently heads its only attainment table
*"Current attainment (April 2026 actuals)"* — so you will see *"April 2026 — five months old"*, not
*"current"*.

**3. If two of your sources disagree, it reports both and stops.** It will not quietly pick one — not
the newer, not the more precise, not the one from the better system. **Choosing between them is a
judgement your data does not contain**, so it names both figures, names where each came from, and
asks you to settle it at source. That is usually the most useful thing in the answer.

**4. It will not tell you a campaign caused a result.** It will tell you two things moved together
over the same period, which is a different and honest claim. Proper attribution needs a defined
model, and Daxko's is written down as *"multi-touch, time-decay weighted"* with the credit split, the
window and the reporting dashboard **all still marked awaiting input**. Until those are filled in,
nobody can honestly attribute — so it says so instead of pretending.

**And it shows its arithmetic.** Not *"39.5% of target"* but *"$10,240,700 ÷ $25,900,000 = 39.5%"*.
If you cannot re-do the sum, you cannot check the claim.

---

## What it will NOT do

| Ask | Who owns it |
|---|---|
| Set up tracking — GA4, GTM, UTMs, events, conversions, attribution | `daxko-analytics-tracking` |
| Anything about one page, or anything where you paste a URL | `daxko-page-cro` |
| Company financials, budget versus actuals, board or CFO reporting | `netsuite-finance-analyst` |
| A traffic drop or lost rankings treated as a search problem | `daxko-seo-audit` |
| Whether variant B is significant yet | `daxko-ab-test-setup` |
| Defining funnel stages, MQL/SQL criteria, lead scoring | `daxko-revops` |
| Ad spend, bidding, return on ad spend, creative performance | `daxko-paid-ads`, `daxko-ad-creative` |
| A spreadsheet, a deck or a document | `xlsx`, `pptx`, `ppt-designer`, `docx` |
| An interactive dashboard or KPI cards | `data:build-dashboard` |
| Turning the findings into QBR slides | **Agent 72 — Executive Insight Summarizer** |
| Deciding what to do about the numbers | **Agent 2 — OKR Copilot**, or your market strategist |
| Moving spend between campaigns | **Agent 71 — Budget Reallocation** |

It also declines non-marketing material — code, legal or contract text, HR documents.

🔴 **And it stops if your export contains personal data** — names, email addresses, phone numbers,
individual user IDs, IP addresses. It tells you which **field** made it stop, without repeating any
of the values, and asks for an aggregated version. Totals are all it needs; it never needs a row
about a person.

**Three more things it never does:** it watches nothing over time (it runs when you ask, and only
then, so it will never "flag this next month"), it writes into no system — no dashboard, no CRM, no
file — and it does not decide what Daxko should do. It tells you what the numbers show and what would
have to change to close a gap.

---

## One honest limit worth knowing

**Its output is not brand-checked.** It carries Daxko's objectives and performance definitions, but
not the brand guidelines or the banned-words list — it writes analysis, not marketing copy. So if an
answer is going to a client, take the next step it offers and send it to **Agent 9 — Brand Guardian**
first.

---

## How to install it

### If it has been installed as a plugin

Nothing to do — it is already there. Just paste your numbers and ask.

### If you use claude.ai

1. Abid Siddiqui sends you the skill, or you add the plugin marketplace he gives you
2. In claude.ai, go to **Settings → Capabilities → Skills**
3. Click **Upload skill** and choose the file
4. Start a new chat, paste some numbers, and try one of the requests above

### If you use Claude Code

1. Unzip the skill folder
2. Put the `daxko-marketing-performance` folder into your Claude Code skills directory
3. Restart Claude Code
4. Try one of the requests above

**Either way, the check that it worked:** ask a performance question with data pasted and confirm you
get back a **coverage** statement at the top naming what it did *not* receive, and a **SOURCES** block
at the end. If either is missing, or you see a file-not-found error, tell Abid Siddiqui — that means
something did not travel correctly and he needs to know.

---

## How to report a bad answer

**If it gets something wrong, say so — but send it to Abid Siddiqui.** Send him:

1. What you asked it
2. What it gave you
3. What it should have given you, and why

**Worth reporting above everything else:** any place it told a story across a gap. A claim about the
whole when it only had part. An old figure presented as current. Two numbers that disagreed and only
one appeared. A campaign described as having *caused* something. A result you could not re-check
because the sum was not shown. **Those are this agent's real failure mode** — not made-up numbers,
but a tidy story built out of real ones that did not belong together. The corrections that fix those
are the most valuable entries in the file.

**Also worth reporting:** if it ever fetches data on its own, or offers to. It should not, ever.

**Do not edit your own copy of the skill.** It will be replaced the next time it is updated and your
change will vanish without a trace — and you would be the only person with the fix.

Abid Siddiqui records every correction in one place. Those corrections are bundled into the next
version, so **everyone** gets them. It works in the other direction too: if it gets something right
that you expected it to get wrong, tell him as well, so a later change does not undo it.

---

## What is inside it

| Folder | What is in it |
|---|---|
| `SKILL.md` | The instructions the agent follows, including the six laws that govern every answer |
| `references/` | The bundled Daxko documents it reads, plus `MANIFEST.md` recording where each came from, its checksum and its date |
| `templates/` | The output shapes — one spine, three sizes |
| `examples/` | One fully grounded answer showing the standard, and one deliberately bad one with all twenty-three faults annotated |

**A note on how the knowledge works.** The documents inside this skill are a **snapshot**, taken the
day it was published. The live versions live in Abid Siddiqui's Agent HQ folder. When they change, he
republishes and you get the update. Your copy is read-only by design — that is what keeps everyone
reading from the same definitions.

Every answer tells you the date of each document it used, in the SOURCES block. If a date looks older
than you expected, ask Abid Siddiqui whether an update is due.

---

## Questions

- **About this agent, an update, or a bad answer** → Abid Siddiqui
- **About what a KPI means or how a KR is defined** → the market's cross-functional team, named in
  `references/okrs-and-priorities.md`
- **About Daxko brand voice, if an answer is going to a client** → Anna Klement, Communications Manager
