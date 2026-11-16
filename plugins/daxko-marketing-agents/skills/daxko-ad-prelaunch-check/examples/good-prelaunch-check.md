# Example — a GOOD answer (shape only)

> **Never quote a fact from this file.** It shows the shape and standard. Every campaign fact in a real answer comes from what the person pasted or pulled with permission; every Daxko rule from `references/`. Names here are obviously fake; numbers are placeholders.

**SCOPE** — Google Ads Search · client: Testford Valley YMCA (as named) · campaign: `tvy-search-[season]` (as pasted) · pasted: settings, brief and naming convention ("lower-case, hyphens only, utm_campaign equals the campaign name") · pulled: none — No connector was used · assumed: nothing.

**DRAFT — needs the campaign owner before anything goes live**

**VERDICT: NO-GO** — 3 Fix, 1 Not given.

| # | Area | What it should be (as pasted) | What it is (as pasted) | Result | Fix in words |
|---|---|---|---|---|---|
| 1 | Naming | "lower-case, hyphens only" | `tvy-search-[season]` | Pass | — |
| 2 | UTM — Ad 1 | utm_campaign = campaign name, lower-case | `utm_source=google&utm_medium=cpc&utm_campaign=tvy-search-[season]` | Pass | — |
| 2 | UTM — Ad 2 | same | `utm_source=Google&utm_medium=CPC&utm_campaign=TVY_Search` | Fix | Lower-case the source and medium; set utm_campaign to the campaign name with hyphens |
| 3 | Conversion tracking | — | not in the paste | Not given | Confirm which conversion action this campaign counts |
| 4 | Landing page URL | `[brief URL]` | same path — not opened, no web access | Pass | Whether it loads → Agent 32 — QA & Testing |
| 5 | Locations | "[N]-mile radius around [place]" | "[2N]-mile radius around [place] plus [another county]" | Fix | Set the radius back to the brief's [N] miles and remove the extra county |
| 6 | Audience | "[audience line]" | "[same]" | Pass | — |
| 7 | Schedule and dates | [start] to [end] | [start] to [end] | Pass | — |
| 8 | Budget | approved [T] | [D]/day × [n] days (both dates counted) = [D × n] vs approved [T] — over by [D × n − T] | Fix | Lower the daily budget; [T] ÷ [n] = [figure] a day fits the total (arithmetic only) |
| 9 | Bid strategy | Not given in brief | "[as stated]" | Not given in brief | Advice on which strategy → `daxko-paid-ads` |
| 10 | Ad text red flags | the client's pasted brief | no line conflicts with the brief | Pass | — |

**FIX LIST** — for the campaign owner: 1. Fix Ad 2's tags as above. 2. Set the radius to the brief's. 3. Lower the daily budget to fit the approved total. 4. Confirm the conversion action, then paste it back.

**INTERNAL NOTES** — arithmetic shown in row 8 · each Fix quotes both pasted lines · client ad text checked against the client's brief only (Daxko's brand rules do not apply to the client's brand) · no personal details were pasted.

**DECLINED** — none asked.

**NOT ON FILE** — conversion tracking · pixel or tag · who signs off — confirm who signs off.

**KEY RESULT** — none on file for Digital Services work; nearest only: "GRR — Nonprofit | 93.9%" (Objective 1).

**NEXT STEP** — Paste the corrected settings and I'll re-check them.

**SOURCES** — `ai-use-rules.md` (in full) · `okrs-and-priorities.md` (search) · each `as_of` from MANIFEST · corrections file read · settings, brief and convention as pasted · No connector was used · SKILL VERSION: 1.9.0 · No web search was used. Nothing was sent, scheduled, published or changed.

**Why this is good:** every Result cites the pasted line it compared; the budget math is shown, not described; the unknown is "Not given", not assumed; the landing page is "not opened"; the verdict follows the rule (any Fix → NO-GO); the FIX LIST is steps for a human — nothing was launched, edited or re-budgeted.
