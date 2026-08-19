> **SOURCE FILE:** `Downloads/daxko-visual-designer 2/references/brand-patterns.md`  ·  **LAST UPDATED:** 2026-03-25 (file date — no "last updated" line stated inside the document)  ·  **Placed in Agent HQ:** 2026-08-11
>
> ✅ **VERIFIED 2026-08-14.** These files did not come from `drop-your-updated-files-here`, but they have been checked byte-for-byte against the `daxko-brand-design-system` skill that is live in Abid Siddiqui's Daxko claude.ai account, and they are IDENTICAL. Confirmed correct by Abid Siddiqui. Full provenance in `visual-brand/INDEX.md`.

# Daxko Brand Pattern Library

The Daxko brand uses two pattern families as decorative background and overlay elements. Patterns add texture and visual rhythm without overpowering content.

---

## Pattern Families

### 1. Small Grid (Dense Directional)

A tight grid of small angular triangle/chevron shapes arranged in a uniform diagonal pattern. Each shape is identical in size. Available in two directions and two color variants.

**Variants:**
| Name | Direction | Color Variant |
|------|-----------|--------------|
| Small Grid ↗️ Light | Diagonals pointing upper-right | Light (`#F0F0F0`) |
| Small Grid ↗️ Dark | Diagonals pointing upper-right | Dark (`#262626`) |
| Small Grid ↖️ Light | Diagonals pointing upper-left | Light (`#F0F0F0`) |
| Small Grid ↖️ Dark | Diagonals pointing upper-left | Dark (`#262626`) |

**Use for:**
- Background texture on light cards and email banners (Light variant at 10–20% opacity)
- Background texture on dark slides and gradient overlays (Dark variant at 15–25% opacity)
- The email banner image (Image 3) uses the Light variant as the background pattern

### 2. Random Grid Fade (Dispersed / Irregular)

A looser arrangement of irregular angular shapes that fades in intensity from one corner. Shapes vary in size and density. This creates a "dispersing" visual effect.

**Variants:**
| Name | Fade Direction | Color Variant |
|------|---------------|--------------|
| Random Grid Light Fade ↗️ | Dense at lower-left, fades toward upper-right | Light (`#F0F0F0`) |
| Random Grid Light Fade ↖️ | Dense at lower-right, fades toward upper-left | Light (`#F0F0F0`) |
| Random Grid Light Fade ⬆️ | Dense at bottom, fades toward top | Light (`#F0F0F0`) |
| Random Grid Dark Fade ↗️ | Dense at lower-left, fades toward upper-right | Dark (`#262626`) |
| Random Grid Dark Fade ↖️ | Dense at lower-right, fades toward upper-left | Dark (`#262626`) |
| Random Grid Dark Fade ⬆️ | Dense at bottom, fades toward top | Dark (`#262626`) |

**Use for:**
- Corner accent patterns on stats slides (see Image 2 — top-right corner cluster)
- Slide header/footer decoration
- Social post backgrounds with subtle depth

---

## Opacity Rules

| Context | Opacity Range |
|---------|--------------|
| Under text content | 10–15% |
| Decorative area (no text over it) | 15–30% |
| Hard maximum | 30% |
| NEVER exceed | 30% |

---

## SVG Implementation

### Small Grid ↗️ Light (CSS background-image)

The Small Grid pattern uses small ↗️-pointing triangular shapes at ~66px spacing, filled `#F0F0F0`:

```css
/* CSS background-image version — tile this pattern */
.pattern-small-grid-light {
  background-image: url("data:image/svg+xml,%3Csvg width='66' height='66' viewBox='0 0 66 66' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M49 10L57 18l2 2c1 1 0.5 2.5-1 2.5H42c-2.8 0-5-2.2-5-5V2C37 0.5 38.5 0 49 10Z' fill='%23F0F0F0'/%3E%3C/svg%3E");
  background-repeat: repeat;
  opacity: 0.15;
}
```

### Inline SVG Pattern (embed directly)

For more precise control (e.g., in HTML assets), embed the SVG directly with `opacity` set on the element:

```html
<!-- Light Small Grid overlay — position absolute over content -->
<div class="pattern-overlay" style="
  position: absolute;
  top: 0; left: 0; right: 0; bottom: 0;
  background-image: url('path/to/Small Grid ↗️ Light.svg');
  background-repeat: repeat;
  background-size: 66px 66px;
  opacity: 0.12;
  pointer-events: none;
  z-index: 1;
"></div>
```

### Inline SVG for Random Grid Fade ↗️ (as overlay)

The Random Grid Fade is best used as a placed SVG image (not tiled), sized to cover the desired region:

```html
<!-- Random Grid Fade — top-right corner decoration -->
<img src="path/to/Random Grid Light Fade ↗️.svg"
     style="
       position: absolute;
       top: 0; right: 0;
       width: 400px; height: 400px;
       opacity: 0.15;
       pointer-events: none;
     "
     alt="" />
```

### Inline Pattern as CSS `currentColor`

To dynamically colorize a pattern to match a brand color, use SVG with `fill="currentColor"`:

```html
<div style="color: #E8236B; opacity: 0.12;">
  <svg viewBox="0 0 100 100" style="position:absolute; top:0; right:0; width:300px;">
    <!-- pattern paths with fill="currentColor" -->
  </svg>
</div>
```

---

## Pattern + Shape Cluster (Slide Top-Right Accent)

The production stats slide (Image 2) uses a specific shape cluster in the top-right corner. This is NOT the tileable grid pattern — it's a custom arrangement of small ↗️ triangles:

```html
<!-- Stats slide top-right shape cluster -->
<div style="position:absolute; top:24px; right:24px; width:220px; height:120px; overflow:hidden;">
  <!-- Row 1 — 6 shapes -->
  <svg style="position:absolute; top:0; right:0; width:180px; height:100px;" viewBox="0 0 180 100">
    <!-- Row of 6 small ↗️ triangles, Core color, varying opacity -->
    <!-- Outer shapes lighter, inner shapes darker -->
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#B81CB5" opacity="0.5" transform="translate(0,0)"/>
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#B81CB5" opacity="0.6" transform="translate(32,0)"/>
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#B81CB5" opacity="0.7" transform="translate(64,0)"/>
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#7B2D8B" opacity="0.8" transform="translate(96,0)"/>
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#7B2D8B" opacity="0.9" transform="translate(128,0)"/>

    <!-- Row 2 — 5 shapes, shifted right by 1 shape width -->
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#B81CB5" opacity="0.4" transform="translate(32,36)"/>
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#B81CB5" opacity="0.5" transform="translate(64,36)"/>
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#B81CB5" opacity="0.65" transform="translate(96,36)"/>
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#7B2D8B" opacity="0.8" transform="translate(128,36)"/>

    <!-- Row 3 — 4 shapes -->
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#B81CB5" opacity="0.35" transform="translate(64,72)"/>
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#B81CB5" opacity="0.5" transform="translate(96,72)"/>
    <path d="M0 30L25 5l2-2c2-2 5-1 5 2V22c0 6.6-5.4 12-12 12H3C0 34-1 32 0 30Z"
          fill="#7B2D8B" opacity="0.65" transform="translate(128,72)"/>
  </svg>
</div>
```

---

## Pattern Selection Guide

| Asset Type | Recommended Pattern |
|------------|-------------------|
| Light background card/email | Small Grid ↗️ Light at 12% opacity |
| Dark/gradient slide | Small Grid ↗️ Dark at 15% opacity |
| Stats/data slide | Random Grid shape cluster (top-right corner) |
| Portrait card (white BG) | Small Grid Light at 10%, full coverage |
| Portrait card (colored BG) | No pattern, or very subtle small grid at 8% |
| Social post (gradient) | No pattern needed if gradient is strong |
| One-pager / flyer | Random Grid Fade corner accent |

---

## pptxgenjs Implementation

```javascript
// Background pattern on a slide
slide.addImage({
  path: 'path/to/Small Grid ↗️ Light.svg',  // or PNG
  x: 0, y: 0,
  w: '100%', h: '100%',
  transparency: 85,  // 85% transparent = 15% opacity
});

// Corner pattern cluster (top-right)
slide.addImage({
  path: 'path/to/Random Grid Light Fade ↗️.svg',
  x: 8.0, y: 0,    // position at right side
  w: 3.5, h: 2.5,
  transparency: 80,  // 20% opacity
});
```
