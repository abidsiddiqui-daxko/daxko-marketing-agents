> **SOURCE FILE:** `Downloads/daxko new logo brand system files/daxko-brand-design-v2/references/logo-guidelines.md`  ·  **LAST UPDATED:** 2026-05-28 (file date — no "last updated" line stated inside the document)  ·  **Placed in Agent HQ:** 2026-08-11
>
> ✅ **VERIFIED 2026-08-14.** These files did not come from `drop-your-updated-files-here`, but they have been checked byte-for-byte against the `daxko-brand-design-system` skill that is live in Abid Siddiqui's Daxko claude.ai account, and they are IDENTICAL. Confirmed correct by Abid Siddiqui. Full provenance in `visual-brand/INDEX.md`.

> 🟢 **TYPOGRAPHY CORRECTED 2026-09-02.** Söhne references in this file were replaced with **Barlow** (Arial as web-safe fallback only). Ruling: Clint Malson — *"Barlow is the correct font. Use the Daxko Brand Standards as your guide"* (Daxko Brand Standards, live.standards.site/daxko2025). This closes open decision **D14** in `registry/DECISIONS.md`. Söhne is no longer permitted anywhere, including the product-lockup exception previously carried in `logo-guidelines.md`.

# Daxko Logo Guidelines

## Purpose

This reference file defines how Claude must handle Daxko logo placement when generating brand-compliant HTML, CSS, and SVG marketing assets. All rules are derived from the official Daxko brand standards (https://live.standards.site/daxko2025/).

**Important:** Claude does not have access to the actual logo files (.svg or .png). All generated templates must include a placeholder comment `<!-- LOGO -->` and an `<img>` tag with a `src` attribute that the user will replace with the correct file path. Never attempt to draw, recreate, or approximate the Daxko logo using CSS shapes, SVG paths, or text styling.

---

## The Daxko X Mark

The Daxko icon — called the "X mark" — is a pinwheel shape made of four rounded, petal-like triangles that meet at the center. It appears in every Daxko logo lockup (both the primary Daxko logo and all product-specific logos). The X mark is the single most recognizable element of the Daxko visual identity.

### X Mark Petal Colors

The four petals each have a distinct brand color. Their positions (when the mark is oriented upright):

| Position | Color Name | Hex | Notes |
|----------|-----------|-----|-------|
| **Top** | Orange / Amber | `#EFAD1C` | Banana Pudding from the Brand Fun Colors palette |
| **Right** | Purple | `#B81CB5` | Matches the Vitality gradient start color |
| **Bottom** | Blue | `#2EAAFF` | Agility Light |
| **Left** | Pink / Magenta | `#E8236B` | Matches the Vitality gradient end / Warning color |

### X Mark Rules

- The X mark colors are **fixed** — they do not change based on context, background, or product.
- The petal colors are always the same regardless of which color variant (full-color, white, black) the accompanying wordmark uses.
- **Exception for single-color variants:** In monochrome white-reversed or black logo variants, ALL petals render in white or black respectively (the multi-color version is preferred whenever possible).
- The petals have soft, rounded edges — they are not sharp triangles. Each petal curves inward at the center and outward at the tip.
- There is a small gap/white space between each petal at the center of the X mark.
- The X mark must maintain a **1:1 aspect ratio** — it is always square.

---

## Logo Variants

Daxko provides two categories of logo, each with multiple color variants. Choose the correct one based on context.

### Daxko Primary Logo

The primary logo consists of the **X mark + "daxko" wordmark** in a horizontal lockup. Use the primary logo when **multiple solutions appear together** in a single asset (e.g., a corporate landing page, a multi-product brochure, a general brand awareness piece). When the primary logo is used, write out the solution name separately in body text or a subheading rather than relying on a solution-specific logo.

### Product-Specific Logos (Solution Logos)

Product logos follow a consistent lockup format: **X mark + "daxko" parent text + product name**. The structure is:

```
[X Mark]  daxko
          product name
```

- The X mark is positioned to the left of the text block.
- "daxko" appears in a lighter/smaller weight above the product name.
- The product name appears below "daxko" in a heavier/larger weight.
- Both text lines are left-aligned to each other.

Use product logos in **single-product contexts** where the asset is dedicated to one product. These are appropriate for product login screens, product-specific landing pages, and single-product campaigns. Each product that requires its own login should use its solution logo.

### Known Daxko Products

| Product Name | Lockup Text |
|---|---|
| Club Automation | daxko / club automation |
| Core | daxko / core |
| Engage | daxko / engage |
| Engage Pro | daxko / engage pro |
| Zenplanner | daxko / zenplanner |
| Operations | daxko / operations |

### Color Variants

Each logo category comes in three color variants:

| Variant | File Suffix Convention | X Mark Treatment | Wordmark Treatment | Usage |
|---|---|---|---|---|
| **Full Color** | `-full-color` | Multi-color petals (orange, purple, blue, pink) | Dark gray/charcoal text | On white or very light neutral backgrounds only |
| **White Reversed** | `-white` | Multi-color petals (preferred) or all-white petals | White text | On dark backgrounds, brand color backgrounds, or photography |
| **Black** | `-black` | All-black petals | Black text | On light backgrounds where full color is not available or appropriate |

---

## Clear Space Rules

Never crowd the logo. All surrounding elements must respect a minimum clear space zone to preserve brand consistency and visual impact.

### Formula

- **Reference unit:** The height of the lowercase "d" in the Daxko wordmark.
- At standard display size, this reference height is approximately **90px**.
- **Minimum clear space on all four sides:** 25% of the total logo height.

For example, if the logo is rendered at 120px tall, the clear space on every side must be at least 30px (120 * 0.25).

### CSS Implementation of Clear Space

Apply clear space using padding on the logo container, not margin on the image itself. This ensures the zone is enforced regardless of surrounding layout.

```css
.daxko-logo-container {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  /* Clear space: 25% of logo height on all sides.
     For a logo rendered at 120px height, padding = 30px.
     Adjust padding proportionally when logo size changes. */
  padding: 25%;
  box-sizing: content-box;
}

.daxko-logo-container img {
  display: block;
  width: 100%;
  height: auto;
  max-width: 100%;
}
```

When using a fixed-size logo, compute the padding explicitly:

```css
/* Example: logo displayed at 48px height */
.daxko-logo-container--fixed {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 12px; /* 48px * 0.25 = 12px */
  box-sizing: content-box;
}

.daxko-logo-container--fixed img {
  display: block;
  height: 48px;
  width: auto;
}
```

---

## Minimum Sizes

The logo must never be rendered smaller than the following thresholds:

| Medium | Minimum Width |
|---|---|
| **Digital (screen)** | 80px |
| **Print** | 1 inch (72pt) |

### Aspect Ratio

The Daxko logo has an approximate aspect ratio of **3:1** (width to height). Always maintain the original proportions. Never set both `width` and `height` to fixed values that would distort the ratio; set one dimension and let the other scale automatically.

```css
/* Correct: set width, let height scale */
.daxko-logo-container img {
  width: 180px;
  height: auto;
}

/* Also correct: set height, let width scale */
.daxko-logo-container img {
  height: 60px;
  width: auto;
}

/* WRONG: setting both breaks the aspect ratio */
.daxko-logo-container img {
  width: 200px;
  height: 100px; /* DO NOT do this */
}
```

---

## Background Rules

The background behind the logo determines which color variant to use.

| Background Type | Logo Variant | Additional Notes |
|---|---|---|
| **White (#FFFFFF)** | Full Color | Use 6-column width container. Optionally include a 1px border stroke for contained placement. |
| **Light neutral** | Full Color or Black | Full color preferred; black acceptable if color reproduction is limited. |
| **Black or dark backgrounds** | White Reversed | Overlay opacity must be 100% (fully opaque container). |
| **Brand color: Vitality 700 (#C90D4C)** | White Reversed | Ensure the color is exact; do not lighten or darken. |
| **Brand color: Agility Dark (#0070D1)** | White Reversed | Ensure the color is exact; do not lighten or darken. |
| **Photography / image backgrounds** | White Reversed | The image region behind the logo must provide a minimum contrast ratio of 4.5:1 against white. If contrast is insufficient, add a semi-transparent dark overlay behind the logo area. |

### CSS for Contained Placement on White

```css
.daxko-logo-container--contained {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 12px; /* adjust per clear space formula */
  background-color: #FFFFFF;
  border: 1px solid #E0E0E0;
  box-sizing: content-box;
}
```

### CSS for Logo on Photography

```css
.daxko-logo-container--overlay {
  position: relative;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 12px; /* adjust per clear space formula */
  box-sizing: content-box;
}

/* Optional dark overlay to guarantee contrast */
.daxko-logo-container--overlay::before {
  content: "";
  position: absolute;
  inset: 0;
  background-color: rgba(0, 0, 0, 0.45);
  border-radius: inherit;
  z-index: 0;
}

.daxko-logo-container--overlay img {
  position: relative;
  z-index: 1;
}
```

---

## Partner Lockups

When the Daxko logo appears alongside a partner logo, use one of two approved layouts.

### Horizontal Lockup

```
[ Daxko Logo ]  |  [ Partner Logo ]
```

- Daxko logo is positioned on the **left**.
- A vertical divider line separates the two logos.
- Partner logo is positioned on the **right**.
- Both logos are **vertically centered** on the divider line.
- The Daxko logo must be **equal to or larger than** the partner logo.
- Clear space between logos (including the divider) must be at least **2x the standard clear space** (i.e., 50% of the Daxko logo height).

```css
.daxko-partner-lockup--horizontal {
  display: inline-flex;
  align-items: center;
  gap: 0; /* gap is handled by the divider padding */
}

.daxko-partner-lockup--horizontal .daxko-logo-container {
  padding-right: 24px; /* 2x clear space */
}

.daxko-partner-lockup--horizontal .lockup-divider {
  width: 1px;
  height: 48px; /* match logo height */
  background-color: #CCCCCC;
  flex-shrink: 0;
}

.daxko-partner-lockup--horizontal .partner-logo-container {
  padding-left: 24px; /* 2x clear space */
}
```

### Vertical Lockup

```
[ Daxko Logo ]
      ---
[ Partner Logo ]
```

- Daxko logo is positioned on **top**.
- A horizontal divider line separates the two logos.
- Partner logo is positioned on the **bottom**.
- Both logos are **horizontally centered** on the divider line.
- Same sizing and spacing rules as horizontal: Daxko logo must be equal to or larger, 2x clear space between logos.

```css
.daxko-partner-lockup--vertical {
  display: inline-flex;
  flex-direction: column;
  align-items: center;
  gap: 0;
}

.daxko-partner-lockup--vertical .daxko-logo-container {
  padding-bottom: 24px; /* 2x clear space */
}

.daxko-partner-lockup--vertical .lockup-divider {
  height: 1px;
  width: 120px; /* match logo width */
  background-color: #CCCCCC;
  flex-shrink: 0;
}

.daxko-partner-lockup--vertical .partner-logo-container {
  padding-top: 24px; /* 2x clear space */
}
```

---

## CSS Implementation

Below is a consolidated CSS block that Claude should include (or adapt) whenever generating an asset that contains the Daxko logo.

```css
/* ============================================
   DAXKO LOGO SYSTEM
   ============================================ */

/* Base logo container — enforces clear space */
.daxko-logo-container {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  box-sizing: content-box;
}

/* Clear space via padding (adjust values per logo size) */
.daxko-logo-container--sm  { padding: 5px;  } /* logo height ~20px, 20*0.25=5   */
.daxko-logo-container--md  { padding: 12px; } /* logo height ~48px, 48*0.25=12  */
.daxko-logo-container--lg  { padding: 20px; } /* logo height ~80px, 80*0.25=20  */
.daxko-logo-container--xl  { padding: 30px; } /* logo height ~120px, 120*0.25=30 */

/* Logo image defaults */
.daxko-logo-container img {
  display: block;
  height: auto;
  width: auto;
  max-width: 100%;
}

/* Minimum size enforcement */
.daxko-logo-container img {
  min-width: 80px; /* digital minimum */
}

/* Contained placement (white bg, border) */
.daxko-logo-container--contained {
  background-color: #FFFFFF;
  border: 1px solid #E0E0E0;
}

/* Dark background placement */
.daxko-logo-container--on-dark {
  background-color: transparent;
}

/* Photography overlay placement */
.daxko-logo-container--on-photo {
  position: relative;
}

.daxko-logo-container--on-photo::before {
  content: "";
  position: absolute;
  inset: 0;
  background-color: rgba(0, 0, 0, 0.45);
  border-radius: inherit;
  z-index: 0;
}

.daxko-logo-container--on-photo img {
  position: relative;
  z-index: 1;
}

/* ============================================
   PARTNER LOCKUPS
   ============================================ */

/* Horizontal */
.daxko-partner-lockup--horizontal {
  display: inline-flex;
  align-items: center;
}

.daxko-partner-lockup--horizontal .lockup-divider {
  width: 1px;
  align-self: stretch;
  background-color: #CCCCCC;
  flex-shrink: 0;
  margin: 0 24px; /* 2x standard clear space */
}

/* Vertical */
.daxko-partner-lockup--vertical {
  display: inline-flex;
  flex-direction: column;
  align-items: center;
}

.daxko-partner-lockup--vertical .lockup-divider {
  height: 1px;
  width: 80%;
  background-color: #CCCCCC;
  flex-shrink: 0;
  margin: 24px 0; /* 2x standard clear space */
}
```

---

## HTML Template Snippet

When generating HTML templates, use the following pattern to mark where the Daxko logo should appear. The user will replace the `src` value with the correct logo file path.

### Standard Logo Placement

```html
<!-- LOGO -->
<div class="daxko-logo-container daxko-logo-container--md">
  <img
    src="[REPLACE_WITH_LOGO_PATH]"
    alt="Daxko"
    width="180"
    height="60"
  />
</div>
```

### Logo on Dark Background

```html
<!-- LOGO -->
<div class="daxko-logo-container daxko-logo-container--md daxko-logo-container--on-dark">
  <img
    src="[REPLACE_WITH_WHITE_LOGO_PATH]"
    alt="Daxko"
    width="180"
    height="60"
  />
</div>
```

### Logo on Photography

```html
<!-- LOGO -->
<div class="daxko-logo-container daxko-logo-container--md daxko-logo-container--on-photo">
  <img
    src="[REPLACE_WITH_WHITE_LOGO_PATH]"
    alt="Daxko"
    width="180"
    height="60"
  />
</div>
```

### Horizontal Partner Lockup

```html
<!-- LOGO: PARTNER LOCKUP -->
<div class="daxko-partner-lockup--horizontal">
  <div class="daxko-logo-container daxko-logo-container--md">
    <img
      src="[REPLACE_WITH_DAXKO_LOGO_PATH]"
      alt="Daxko"
      width="180"
      height="60"
    />
  </div>
  <div class="lockup-divider" aria-hidden="true"></div>
  <div class="partner-logo-container">
    <img
      src="[REPLACE_WITH_PARTNER_LOGO_PATH]"
      alt="[Partner Name]"
      height="60"
      width="auto"
    />
  </div>
</div>
```

### Vertical Partner Lockup

```html
<!-- LOGO: PARTNER LOCKUP -->
<div class="daxko-partner-lockup--vertical">
  <div class="daxko-logo-container daxko-logo-container--md">
    <img
      src="[REPLACE_WITH_DAXKO_LOGO_PATH]"
      alt="Daxko"
      width="180"
      height="60"
    />
  </div>
  <div class="lockup-divider" aria-hidden="true"></div>
  <div class="partner-logo-container">
    <img
      src="[REPLACE_WITH_PARTNER_LOGO_PATH]"
      alt="[Partner Name]"
      width="180"
      height="auto"
    />
  </div>
</div>
```

---

## Logo Implementation in Generated Assets

**Critical rule:** Never attempt to draw, recreate, or approximate the Daxko logo (including the X mark) using CSS shapes, SVG paths, or text styling. Always use the actual logo image files provided by the brand team.

All generated templates must include an `<img>` tag with a `src` attribute set to `[REPLACE_WITH_LOGO_PATH]` (or `[REPLACE_WITH_PRODUCT_LOGO_PATH]` for product-specific assets). The user will replace this placeholder with the correct file path.

### Primary Logo Placeholder

```html
<!-- LOGO — Replace [REPLACE_WITH_LOGO_PATH] with the actual Daxko logo file.
     Use full-color variant on white/light backgrounds.
     Use white reversed variant on dark/colored backgrounds.
     Never attempt to recreate the logo with CSS shapes or SVG paths. -->
<div class="daxko-logo-container">
  <img src="[REPLACE_WITH_LOGO_PATH]" alt="Daxko" />
</div>
```

### Product Logo Placeholder

```html
<!-- PRODUCT LOGO — Replace [REPLACE_WITH_PRODUCT_LOGO_PATH] with the actual product logo file.
     Product logos follow the lockup format: X mark + "daxko" / "product name".
     Use white reversed variant on dark/colored backgrounds.
     Never attempt to recreate the logo with CSS shapes or SVG paths. -->
<div class="daxko-logo-container">
  <img src="[REPLACE_WITH_PRODUCT_LOGO_PATH]" alt="[Product Name] by Daxko" />
</div>
```

---

## Don'ts

Claude must **never** do any of the following when handling the Daxko logo:

1. **Don't stretch or distort.** Always maintain the original aspect ratio (approximately 3:1 for the full lockup, 1:1 for the X mark alone). Never set both width and height to arbitrary values.
2. **Don't rotate.** The logo must always appear at 0 degrees. No CSS `transform: rotate()` or SVG rotation.
3. **Don't recolor the X mark petals.** The four petal colors (orange `#EFAD1C`, purple `#B81CB5`, blue `#2EAAFF`, pink `#E8236B`) are fixed. The only exception is monochrome variants where all petals are white or all are black.
4. **Don't add shadows, gradients, or effects.** No `box-shadow`, `text-shadow`, `drop-shadow()`, gradient overlays, glow effects, or any other visual treatment on the logo itself.
5. **Don't crop any part of the logo.** Never use `overflow: hidden` on a container that would clip the logo. Never use `object-fit: cover` on the logo image.
6. **Don't place on busy or cluttered backgrounds.** If the background has complex imagery, patterns, or multiple competing colors, add a solid or semi-transparent overlay behind the logo to ensure legibility.
7. **Don't render smaller than minimum size.** The logo must be at least 80px wide on screen. The X mark alone must be at least 20px. If layout constraints would force it below this threshold, omit the logo or restructure the layout.
8. **Don't alter the logo typeface.** Never attempt to recreate the "daxko" wordmark with a custom font rendering in the full logo lockup. The wordmark is set in **Barlow**. When using the product lockup HTML pattern, set the text portion in Barlow SemiBold 600 — Söhne is not permitted (corrected 2026-09-02).
9. **Don't violate clear space.** No element (text, images, borders, decorations) may encroach within the 25%-of-logo-height clear space zone on any side.
10. **Don't invent product names.** Only use product names from the Known Daxko Products table. If a product name is not listed, ask the user to confirm it.
11. **Don't create custom X mark icons for products.** Every Daxko product uses the same X mark. There are no product-specific icons (no "Z" for Zenplanner, no "C" for Core, etc.). The X mark is universal across all products.
12. **Don't swap petal positions.** The petal order (top=orange, right=purple, bottom=blue, left=pink) is fixed. Never rearrange the petals.
