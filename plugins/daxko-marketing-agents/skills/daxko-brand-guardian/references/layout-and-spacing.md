> **SOURCE FILE:** `Downloads/daxko new logo brand system files/daxko-brand-design-v2/references/layout-and-spacing.md`  ·  **LAST UPDATED:** 2026-05-28 (file date — no "last updated" line stated inside the document)  ·  **Placed in Agent HQ:** 2026-08-11
>
> ✅ **VERIFIED 2026-08-14.** These files did not come from `drop-your-updated-files-here`, but they have been checked byte-for-byte against the `daxko-brand-design-system` skill that is live in Abid Siddiqui's Daxko claude.ai account, and they are IDENTICAL. Confirmed correct by Abid Siddiqui. Full provenance in `visual-brand/INDEX.md`.

> 🟢 **TYPOGRAPHY CORRECTED 2026-09-02.** Söhne references in this file were replaced with **Barlow** (Arial as web-safe fallback only). Ruling: Clint Malson — *"Barlow is the correct font. Use the Daxko Brand Standards as your guide"* (Daxko Brand Standards, live.standards.site/daxko2025). This closes open decision **D14** in `registry/DECISIONS.md`. Söhne is no longer permitted anywhere, including the product-lockup exception previously carried in `logo-guidelines.md`.

# Daxko Brand Design System: Layout and Spacing Reference

**Source:** https://live.standards.site/daxko2025/
**Purpose:** Definitive layout, grid, spacing, and component dimension rules for generating brand-compliant Daxko marketing assets as HTML/CSS. All generated layouts must conform to this specification.

---

## Grid System

Daxko uses a **12-column responsive grid** with a fixed gap and a maximum content width.

### Rules

- The grid is always 12 columns.
- Column gap is always **20px**.
- Maximum content width is **1440px**, centered horizontally with `margin: 0 auto`.
- Content blocks span a defined number of columns: **2, 3, 4, 5, 6, 7, 8, 9** columns depending on the content type.
- Full-width backgrounds extend edge-to-edge; the inner content container is constrained to 1440px.

### Common Column Spans

| Columns | Use Case |
|---------|----------|
| 2       | Buttons, small UI elements, sidebar icons |
| 3       | Cards in a 4-column card grid, thumbnails |
| 4       | Cards in a 3-column card grid, sidebar panels |
| 5       | Asymmetric text/image splits (narrow side) |
| 6       | 50/50 two-column layouts (each side) |
| 7       | Asymmetric text/image splits (wide side) |
| 8       | Primary content column with sidebar |
| 9       | Wide content column with narrow sidebar |
| 12      | Full-width sections, hero banners |

### CSS Grid Implementation

```css
.daxko-grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: 20px;
  max-width: 1440px;
  margin: 0 auto;
  width: 100%;
}

.col-2  { grid-column: span 2; }
.col-3  { grid-column: span 3; }
.col-4  { grid-column: span 4; }
.col-5  { grid-column: span 5; }
.col-6  { grid-column: span 6; }
.col-7  { grid-column: span 7; }
.col-8  { grid-column: span 8; }
.col-9  { grid-column: span 9; }
.col-12 { grid-column: span 12; }
```

---

## Spacing Scale

All spacing in Daxko layouts uses a fixed named scale. Never use arbitrary pixel values outside this scale.

| Token | Value | Use |
|-------|-------|-----|
| `xs`  | 8px   | Tight internal padding, icon gaps |
| `sm`  | 16px  | Inline element spacing, small internal padding |
| `md`  | 24px  | Default element spacing, card internal padding |
| `lg`  | 40px  | Grouped section spacing, generous internal padding |
| `xl`  | 60px  | Sub-section breaks, large grouped spacing |
| `2xl` | 100px | Major section dividers, top/bottom section padding |

### CSS Custom Properties for Spacing

```css
:root {
  --space-xs: 8px;
  --space-sm: 16px;
  --space-md: 24px;
  --space-lg: 40px;
  --space-xl: 60px;
  --space-2xl: 100px;
}
```

---

## Component Heights

Standard vertical dimensions for major layout sections.

| Component      | Height        | Notes |
|----------------|---------------|-------|
| Standard row   | 520px         | Default height for content rows and feature blocks |
| Section        | 540px-700px   | Flexible range; content determines exact height within range |
| Hero section   | Flexible, minimum 400px | Grows to fit content; never shorter than 400px |

### CSS Custom Properties for Heights

```css
:root {
  --height-row: 520px;
  --height-section-min: 540px;
  --height-section-max: 700px;
  --height-hero-min: 400px;
}
```

---

## Padding Standards

Padding follows a strict hierarchy based on the relationship between elements.

### Hierarchy

| Context                          | Padding/Margin | Token |
|----------------------------------|----------------|-------|
| Adjacent related elements        | 20px           | (grid gap handles this) |
| Container internal padding       | 15px-20px      | `sm` to grid gap |
| Grouped sections                 | 40px-60px      | `lg` to `xl` |
| Major section breaks (top/bottom)| 100px          | `2xl` |

### Rules

1. **Adjacent related elements** (e.g., heading and paragraph, image and caption): Use the grid gap (20px) or `var(--space-sm)` to `var(--space-md)`.
2. **Container internal padding**: Apply 15px-20px inside cards, panels, and boxed components.
3. **Grouped sections** (e.g., a feature block containing a heading, body text, and CTA): Use `var(--space-lg)` (40px) to `var(--space-xl)` (60px) between groups.
4. **Major section dividers** (e.g., between a hero and a feature grid, between two top-level page sections): Use `var(--space-2xl)` (100px) as top and bottom padding on the section wrapper.

---

## Button Specifications

Buttons in the Daxko system have a distinctive flat, square-cornered appearance. This is intentional and must not be altered.

### Visual Spec

| Property         | Value |
|------------------|-------|
| Width            | 2-column span, or `auto` with internal padding |
| Padding          | 15px top/bottom, 20px left/right |
| Background       | `rgba(137, 137, 137, 0.15)` (#898989 at 15% opacity) |
| Hover background | `rgba(137, 137, 137, 0.25)` (#898989 at 25% opacity) |
| Font family      | Barlow SemiBold |
| Font weight      | 600 |
| Font size        | 14px |
| Border radius    | **0** (square corners, intentional) |
| Border           | none |
| Transition       | `background 0.2s ease` |
| Text color       | Inherited from context: white on dark backgrounds, dark on light backgrounds |
| Cursor           | pointer |

### Full CSS Class

```css
.daxko-btn {
  display: inline-block;
  padding: 15px 20px;
  background: rgba(137, 137, 137, 0.15);
  border: none;
  border-radius: 0;
  font-family: 'Barlow', Arial, sans-serif;
  font-weight: 600;
  font-size: 14px;
  color: inherit;
  cursor: pointer;
  transition: background 0.2s ease;
  text-decoration: none;
  line-height: 1;
}

.daxko-btn:hover {
  background: rgba(137, 137, 137, 0.25);
}

/* Context variants */
.daxko-btn--on-dark {
  color: #ffffff;
}

.daxko-btn--on-light {
  color: #1a1a1a;
}
```

---

## CSS Custom Properties (Complete Set)

Combine all custom properties into a single `:root` block in every generated asset.

```css
:root {
  /* Grid */
  --grid-columns: 12;
  --grid-gap: 20px;
  --grid-max-width: 1440px;

  /* Spacing Scale */
  --space-xs: 8px;
  --space-sm: 16px;
  --space-md: 24px;
  --space-lg: 40px;
  --space-xl: 60px;
  --space-2xl: 100px;

  /* Component Heights */
  --height-row: 520px;
  --height-section-min: 540px;
  --height-section-max: 700px;
  --height-hero-min: 400px;

  /* Button */
  --btn-padding-y: 15px;
  --btn-padding-x: 20px;
  --btn-bg: rgba(137, 137, 137, 0.15);
  --btn-bg-hover: rgba(137, 137, 137, 0.25);
  --btn-font-size: 14px;
  --btn-font-weight: 600;
  --btn-radius: 0;
}
```

---

## CSS Implementation (Utility Classes)

Ready-to-use utility classes for grid layout and spacing. Include these in every generated HTML asset.

```css
/* ---- Grid ---- */
.daxko-grid {
  display: grid;
  grid-template-columns: repeat(var(--grid-columns), 1fr);
  gap: var(--grid-gap);
  max-width: var(--grid-max-width);
  margin: 0 auto;
  width: 100%;
}

.col-2  { grid-column: span 2; }
.col-3  { grid-column: span 3; }
.col-4  { grid-column: span 4; }
.col-5  { grid-column: span 5; }
.col-6  { grid-column: span 6; }
.col-7  { grid-column: span 7; }
.col-8  { grid-column: span 8; }
.col-9  { grid-column: span 9; }
.col-12 { grid-column: span 12; }

/* ---- Spacing Utilities ---- */
.mt-xs  { margin-top: var(--space-xs); }
.mt-sm  { margin-top: var(--space-sm); }
.mt-md  { margin-top: var(--space-md); }
.mt-lg  { margin-top: var(--space-lg); }
.mt-xl  { margin-top: var(--space-xl); }
.mt-2xl { margin-top: var(--space-2xl); }

.mb-xs  { margin-bottom: var(--space-xs); }
.mb-sm  { margin-bottom: var(--space-sm); }
.mb-md  { margin-bottom: var(--space-md); }
.mb-lg  { margin-bottom: var(--space-lg); }
.mb-xl  { margin-bottom: var(--space-xl); }
.mb-2xl { margin-bottom: var(--space-2xl); }

.pt-xs  { padding-top: var(--space-xs); }
.pt-sm  { padding-top: var(--space-sm); }
.pt-md  { padding-top: var(--space-md); }
.pt-lg  { padding-top: var(--space-lg); }
.pt-xl  { padding-top: var(--space-xl); }
.pt-2xl { padding-top: var(--space-2xl); }

.pb-xs  { padding-bottom: var(--space-xs); }
.pb-sm  { padding-bottom: var(--space-sm); }
.pb-md  { padding-bottom: var(--space-md); }
.pb-lg  { padding-bottom: var(--space-lg); }
.pb-xl  { padding-bottom: var(--space-xl); }
.pb-2xl { padding-bottom: var(--space-2xl); }

.px-sm  { padding-left: var(--space-sm); padding-right: var(--space-sm); }
.px-md  { padding-left: var(--space-md); padding-right: var(--space-md); }
.px-lg  { padding-left: var(--space-lg); padding-right: var(--space-lg); }

.py-lg  { padding-top: var(--space-lg); padding-bottom: var(--space-lg); }
.py-xl  { padding-top: var(--space-xl); padding-bottom: var(--space-xl); }
.py-2xl { padding-top: var(--space-2xl); padding-bottom: var(--space-2xl); }

.gap-xs  { gap: var(--space-xs); }
.gap-sm  { gap: var(--space-sm); }
.gap-md  { gap: var(--space-md); }
.gap-lg  { gap: var(--space-lg); }

/* ---- Section Wrapper ---- */
.daxko-section {
  padding-top: var(--space-2xl);
  padding-bottom: var(--space-2xl);
}

.daxko-section__inner {
  max-width: var(--grid-max-width);
  margin: 0 auto;
  padding-left: var(--space-sm);
  padding-right: var(--space-sm);
}
```

---

## Layout Patterns

Common layout structures used across Daxko marketing assets. Use these as starting templates.

### Hero Section

Full-width background with centered content. Minimum height 400px.

```html
<section class="daxko-section" style="min-height: var(--height-hero-min); background: #0f1923;">
  <div class="daxko-section__inner">
    <div class="daxko-grid" style="align-items: center; min-height: var(--height-hero-min);">
      <div class="col-7">
        <h1>Hero Headline</h1>
        <p class="mt-md">Supporting text for the hero section.</p>
        <a href="#" class="daxko-btn daxko-btn--on-dark mt-lg">Call to Action</a>
      </div>
      <div class="col-5">
        <!-- Hero image or graphic -->
      </div>
    </div>
  </div>
</section>
```

### Two-Column (50/50)

Equal split for side-by-side content.

```html
<section class="daxko-section">
  <div class="daxko-section__inner">
    <div class="daxko-grid" style="align-items: center; min-height: var(--height-row);">
      <div class="col-6">
        <h2>Section Heading</h2>
        <p class="mt-md">Description text.</p>
        <a href="#" class="daxko-btn daxko-btn--on-light mt-lg">Learn More</a>
      </div>
      <div class="col-6">
        <!-- Image or supporting content -->
      </div>
    </div>
  </div>
</section>
```

### Two-Column (Asymmetric 7/5)

Wider content side with narrower supporting side.

```html
<section class="daxko-section">
  <div class="daxko-section__inner">
    <div class="daxko-grid" style="align-items: center; min-height: var(--height-row);">
      <div class="col-7">
        <h2>Primary Content</h2>
        <p class="mt-md">Detailed explanation or feature description.</p>
      </div>
      <div class="col-5">
        <!-- Supporting visual -->
      </div>
    </div>
  </div>
</section>
```

### Full-Width Content Block

Single column spanning all 12 columns, typically for statements or large callouts.

```html
<section class="daxko-section" style="background: #f5f5f5;">
  <div class="daxko-section__inner" style="text-align: center;">
    <div class="daxko-grid">
      <div class="col-12">
        <h2>Full-Width Statement</h2>
        <p class="mt-md" style="max-width: 720px; margin-left: auto; margin-right: auto;">
          Centered body text constrained for readability.
        </p>
      </div>
    </div>
  </div>
</section>
```

### Card Grid (3-up)

Three equal cards in a row, each spanning 4 columns.

```html
<section class="daxko-section">
  <div class="daxko-section__inner">
    <div class="daxko-grid">
      <div class="col-4" style="padding: var(--space-md);">
        <h3>Card Title</h3>
        <p class="mt-sm">Card description text.</p>
      </div>
      <div class="col-4" style="padding: var(--space-md);">
        <h3>Card Title</h3>
        <p class="mt-sm">Card description text.</p>
      </div>
      <div class="col-4" style="padding: var(--space-md);">
        <h3>Card Title</h3>
        <p class="mt-sm">Card description text.</p>
      </div>
    </div>
  </div>
</section>
```

### Card Grid (4-up)

Four equal cards in a row, each spanning 3 columns.

```html
<section class="daxko-section">
  <div class="daxko-section__inner">
    <div class="daxko-grid">
      <div class="col-3" style="padding: var(--space-sm);">
        <h3>Card Title</h3>
        <p class="mt-sm">Card text.</p>
      </div>
      <div class="col-3" style="padding: var(--space-sm);">
        <h3>Card Title</h3>
        <p class="mt-sm">Card text.</p>
      </div>
      <div class="col-3" style="padding: var(--space-sm);">
        <h3>Card Title</h3>
        <p class="mt-sm">Card text.</p>
      </div>
      <div class="col-3" style="padding: var(--space-sm);">
        <h3>Card Title</h3>
        <p class="mt-sm">Card text.</p>
      </div>
    </div>
  </div>
</section>
```

---

## Don'ts

These rules are non-negotiable. Violating any of them produces an off-brand asset.

1. **No rounded corners on buttons.** `border-radius` must be `0` on all buttons. The square-cornered button is a deliberate Daxko brand decision.
2. **No spacing values outside the defined scale.** Every margin, padding, and gap must map to one of: `8px`, `16px`, `24px`, `40px`, `60px`, `100px`. Never use `10px`, `12px`, `30px`, `50px`, `80px`, or any other arbitrary value.
3. **No content wider than 1440px.** The grid container must always enforce `max-width: 1440px`.
4. **No columns outside the defined spans.** Only use `span 2`, `span 3`, `span 4`, `span 5`, `span 6`, `span 7`, `span 8`, `span 9`, or `span 12`. Never use `span 1`, `span 10`, or `span 11`.
5. **No grid gap other than 20px.** The column gap is fixed at `20px` for the main layout grid. Utility classes like `.gap-sm` are for non-grid flex or internal layouts only.
6. **No section padding smaller than 100px.** Top-level page sections must use `var(--space-2xl)` (100px) for vertical padding. Smaller padding is only for internal element spacing within a section.
7. **No hero section shorter than 400px.** The hero must always meet its minimum height.
8. **No button font size other than 14px at weight 600.** Do not scale buttons up or down. The button style is fixed.
9. **No button borders.** Buttons use background opacity changes for interaction states, not borders or outlines.
10. **No inline styles that contradict the spacing scale or grid rules.** If an inline style is necessary, it must still use values from the defined scale or CSS custom properties.
