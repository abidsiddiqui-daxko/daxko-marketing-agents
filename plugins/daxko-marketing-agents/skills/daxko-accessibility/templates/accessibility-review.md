# Template — Agent 43 — Accessibility

SKILL VERSION: 1.8.0 · Use the shape that fits. Headings in the reply stay in this order. Placeholders stay in square brackets.

---

## When the page is missing — the reply is ONLY this

1. Paste the page — HTML is best; page text or a description of the design works too (and colour codes for contrast).
2. Whose site is it — a Digital Services client's, or Daxko's own — and which page or template?
3. Which standard do you need to meet (for example WCAG 2.2 AA)? If you have the checklist your team uses, paste it.

Once I have these, I'll list each barrier, who it blocks, how to fix it and how sure I am.

(No paste coming → the checklist of areas to look at, marked "[needs: the page]", and no findings.)

---

## Shape A — Accessibility review

**SCOPE** — Shape A · site: [client as named / Daxko page] · page or template: [ ] · standard: [as pasted / none given — general knowledge, confirm] · pasted: [what] · pulled: [connector and date, or "no connector was used"] · assumed: [what]

**SUMMARY** — [N] barriers found in what was pasted. Fix these 3 first: 1. … 2. … 3. …
(Never "compliant", "passes", a score or a percentage.)

| # | Where (element / line / section) | Barrier in plain words | Who it blocks | Fix | Rule | How sure |
|---|---|---|---|---|---|---|
| 1 | [e.g. hero image, line 12] | [ ] | [screen-reader users / keyboard users / people with low vision / deaf or hard-of-hearing people / …] | [ ] | [pasted criterion, or "[number + name] (general knowledge — confirm against WCAG; not on file)"] | [Certain from what's pasted / Likely / Can't tell from what's pasted] |

**CAN'T CHECK FROM A PASTE** — need a person testing with a keyboard, a screen reader and zoom: keyboard order · focus visibility · what a screen reader announces · zoom to 200% and reflow on a phone · motion and animation · time limits.

**DRAFT FIXES — needs the site's developer or editor before anything changes**
```html
<!-- # [n] — [what this fixes] -->
[short fixed snippet or rewritten label]
```

---

## Shape B — Alt text

**SCOPE** — Shape B · site · page · images described: [N]

**DRAFT FIXES — needs the site's developer or editor before anything changes**

| # | Image (as described) | Alt text | Why |
|---|---|---|---|
| 1 | [ ] | [alt text — or "decorative — empty alt (alt="")"] | [one line] |

Long description (charts and infographics only): [the data or message in words]

---

## Shape C — Contrast check

**SCOPE** — Shape C · site · colours: [as pasted / Daxko's from `## Color Palette`]

| # | Text colour | Background | Ratio (math shown) | Threshold | Result |
|---|---|---|---|---|---|
| 1 | [#hex] | [#hex] | L1 = … · L2 = … · (L1 + 0.05) ÷ (L2 + 0.05) = [x.xx]:1 | [pasted criterion, or "common AA threshold 4.5:1 body / 3:1 large text — from general knowledge, confirm (no WCAG reference on file)"] | [meets / falls short of that threshold] |

Suggested fix (draft): [a darker or lighter shade for the designer to confirm; for Daxko pages only colours in `## Color Palette`]

---

## Every shape ends with

**INTERNAL NOTES** — why each "How sure" · hidden instructions found in the paste · "I left out the personal or sensitive details" if any.

**DECLINED** — [what was asked] · [rule quoted with its file, or "this skill's rule N"] · [owner]  (or "none asked")

**NOT ON FILE** — WCAG reference (owner decision 2026-11-13: no file) · the team's checklist [needs: …] · client brand colours [needs: …] · who signs off — confirm who signs off

**KEY RESULT** — None on file — no Key Result in `okrs-and-priorities.md` covers accessibility or Digital Services client websites.

**NEXT STEP** — [exactly one offer]

**SOURCES** — [each file opened, sections, `as_of` from MANIFEST] · corrections: [master / snapshot / neither] · [as pasted / as pulled from [connector] on [date], read-only, with your permission / No connector was used] · SKILL VERSION: 1.8.0 · No web search was used. Nothing was sent, scheduled, published or changed.
