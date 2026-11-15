> **SOURCE FILE:** `Downloads/daxko new logo brand system files/daxko-brand-design-v2/references/typography-system.md`  ·  **LAST UPDATED:** 2026-05-28 (file date — no "last updated" line stated inside the document)  ·  **Placed in Agent HQ:** 2026-08-11
>
> ✅ **VERIFIED 2026-08-14.** These files did not come from `drop-your-updated-files-here`, but they have been checked byte-for-byte against the `daxko-brand-design-system` skill that is live in Abid Siddiqui's Daxko claude.ai account, and they are IDENTICAL. Confirmed correct by Abid Siddiqui. Full provenance in `visual-brand/INDEX.md`.

# Daxko Brand Typography System

## Purpose

This document is the definitive typography reference for generating brand-compliant Daxko marketing assets as HTML/CSS and SVG. All text rendering in generated assets must conform to the specifications below. No exceptions.

**Font Sources:**
- **Barlow** — The sole Daxko brand font. Available from Google Fonts (`https://fonts.google.com/specimen/Barlow`). Web fallback stack: `'Barlow', Arial, sans-serif`

---

## The Daxko Font: Barlow

Barlow is used for all typography — headlines, subheadlines, body copy, captions, CTAs, and UI labels. It is the only permitted font. No other typeface may be used in any Daxko marketing asset.

### Barlow SemiBold (weight 600)

Used for headlines.

### Barlow Regular (weight 400)

Used for subheadlines, body copy, captions, and all supporting text.

### Letter Spacing

- Range: `0px` to `1px` depending on application.
- Headlines: `0px` (default tracking).
- Smaller text and captions: up to `1px` for legibility.

### Text Transform

- **Always `none`.** No all-caps, no uppercase transforms. Ever.
- All text uses **sentence case** (capitalize first word and proper nouns only).

---

## Type Scale Table

Complete reference of every typographic scale in the system:

| Scale Name | Font   | Weight         | Size    | Line Height | Letter Spacing | Use Case                                      |
|-----------|--------|----------------|---------|-------------|----------------|-----------------------------------------------|
| Headline  | Barlow | SemiBold (600) | 80–88pt | 88pt        | 0px            | Hero headlines, primary page titles           |
| Subhead   | Barlow | Regular (400)  | 30pt    | 36pt        | 0px            | Section subheadlines, feature titles          |
| Body      | Barlow | Regular (400)  | 15pt    | 21pt        | 0px            | Paragraphs, descriptions, body copy, captions |

---

## Responsive Scaling

Typography scales down for mobile viewports to maintain readability and visual balance.

### Mobile Adjustments

- **Scaling mode:** fluid, using CSS `clamp()` for smooth transitions between breakpoints.

### Responsive Mapping

| Desktop Scale | Desktop Size | Mobile Size | Mobile Line Height |
|--------------|-------------|-------------|--------------------|
| Headline     | 80–88pt     | 42–48pt     | Fluid              |
| Subhead      | 30pt        | 22pt        | 28pt               |
| Body         | 15pt        | 15pt        | 21pt               |

### Breakpoint

- Mobile styles apply below `768px` viewport width.
- Use `clamp()` for fluid scaling between `375px` and `1280px`.

---

## CSS Custom Properties

Define these custom properties at the `:root` level in all generated assets:

```css
:root {
  /* Font Family */
  --daxko-font: 'Barlow', Arial, sans-serif;

  /* Font Weights */
  --daxko-weight-regular: 400;
  --daxko-weight-semibold: 600;

  /* Type Scale — Sizes */
  --daxko-size-headline: 84pt;     /* midpoint of 80–88pt range */
  --daxko-size-subhead: 30pt;
  --daxko-size-body: 15pt;

  /* Line Heights */
  --daxko-lh-headline: 88pt;
  --daxko-lh-subhead: 36pt;
  --daxko-lh-body: 21pt;

  /* Letter Spacing */
  --daxko-ls-normal: 0px;
  --daxko-ls-wide: 1px;
}
```

---

## CSS Implementation

Ready-to-use CSS classes for all typographic scales. Include these in generated HTML/CSS assets:

```css
/* ============================================
   DAXKO TYPOGRAPHY CLASSES
   ============================================ */

/* --- Headline (Barlow SemiBold) --- */

.daxko-headline {
  font-family: var(--daxko-font);
  font-weight: var(--daxko-weight-semibold);
  font-size: clamp(48pt, 6vw, 84pt);
  line-height: var(--daxko-lh-headline);
  letter-spacing: var(--daxko-ls-normal);
  text-transform: none;
}

/* --- Subhead (Barlow Regular) --- */

.daxko-subhead {
  font-family: var(--daxko-font);
  font-weight: var(--daxko-weight-regular);
  font-size: var(--daxko-size-subhead);
  line-height: var(--daxko-lh-subhead);
  letter-spacing: var(--daxko-ls-normal);
  text-transform: none;
}

/* --- Body (Barlow Regular) --- */

.daxko-body {
  font-family: var(--daxko-font);
  font-weight: var(--daxko-weight-regular);
  font-size: var(--daxko-size-body);
  line-height: var(--daxko-lh-body);
  letter-spacing: var(--daxko-ls-normal);
  text-transform: none;
}

/* --- Responsive Scaling --- */

@media (max-width: 768px) {
  .daxko-headline {
    font-size: clamp(36pt, 8vw, 60pt);
    line-height: 1.1;
  }

  .daxko-subhead {
    font-size: 22pt;
    line-height: 28pt;
  }

  .daxko-body {
    font-size: 15pt;
    line-height: 21pt;
  }
}
```

---

## Usage Rules

### When to Use Barlow SemiBold (600)

- Hero headlines and primary page titles
- CTA button text
- Emphasized labels

### When to Use Barlow Regular (400)

- Subheadlines and section titles
- All body copy
- Captions and metadata
- Navigation items
- Descriptions

### Casing Rules

- **Sentence case for everything.** Capitalize the first word of a headline and proper nouns. Nothing else.
- Example correct: "Grow your community with Daxko"
- Example incorrect: "GROW YOUR COMMUNITY WITH DAXKO"
- Example incorrect: "Grow Your Community With Daxko" (title case)

---

## Don'ts

1. **No fonts other than Barlow.** Sohne, Helvetica, Inter, Roboto, and all other typefaces are not permitted. Arial is the web-safe fallback only — never specify it as the primary font.
2. **No all-caps.** Never apply `text-transform: uppercase` to any element. This includes buttons, labels, navigation, and headlines.
3. **No title case on headlines.** Always sentence case.
4. **No weight values other than 400 and 600.** Do not use light (300), medium (500), bold (700), or black (900) weights.
5. **No negative letter-spacing.** Letter spacing must be between `0px` and `1px`.
6. **No decorative text effects.** No text shadows, outlines, gradients on text, or distortion. Clean, flat typography only.
7. **No sizes outside the defined scale.** Use only the three defined scales (Headline, Subhead, Body). Do not invent intermediate sizes.
8. **No underlined text except for hyperlinks.** Text decoration should only indicate interactive links.
