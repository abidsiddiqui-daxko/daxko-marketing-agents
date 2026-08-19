> **SOURCE FILE:** `Downloads/daxko-visual-designer 2/references/brand-shapes.md`  ·  **LAST UPDATED:** 2026-03-25 (file date — no "last updated" line stated inside the document)  ·  **Placed in Agent HQ:** 2026-08-11
>
> ✅ **VERIFIED 2026-08-14.** These files did not come from `drop-your-updated-files-here`, but they have been checked byte-for-byte against the `daxko-brand-design-system` skill that is live in Abid Siddiqui's Daxko claude.ai account, and they are IDENTICAL. Confirmed correct by Abid Siddiqui. Full provenance in `visual-brand/INDEX.md`.

# Daxko Brand Shape Library

The Daxko brand uses a precise library of geometric shapes: **rounded squares** (rotated 45°, appearing as diamonds) and **corner-cut triangles** (in 8 directional orientations). These are the ONLY shapes used in Daxko brand materials. Never create freehand triangles, custom polygons, or modified versions of these shapes.

---

## Shape Taxonomy

### Shape Types

| Shape | Description |
|-------|-------------|
| **Square** | Rounded-corner square, often used as an outline accent or color block |
| **Triangle** | Corner-cut shape with a large triangle and a small notch cut — comes in 8 compass directions |

### Direction Orientations (Triangles)

Each triangle points to a corner or edge. Use the direction to determine where it should anchor on the design:

| Notation | Points Toward | Best Used At |
|----------|--------------|-------------|
| ↖️ | Upper-left | Bottom-right corner of an asset |
| ↗️ | Upper-right | Bottom-left corner of an asset |
| ↘️ | Lower-right | Upper-left corner of an asset |
| ↙️ | Lower-left | Upper-right corner of an asset |
| ⬆️ | Up | Bottom edge |
| ⬇️ | Down | Top edge |
| ⬅️ | Left | Right edge |
| ➡️ | Right | Left edge |

### Colors

| Color Name | Hex | Brand Family |
|-----------|-----|-------------|
| Vitality | `#E8236B` | Vitality 600 — magenta/pink |
| Core | `#B81CB5` | Core 700 — purple |
| Agility | `#038BED` | Agility 500 — blue |
| Champion | `#FBB03B` | Champion 300 — amber |
| Mode | `#595959` | Flex 600 — gray (dark backgrounds) |

### Styles

| Style | Description |
|-------|-------------|
| **Solid** | Filled with color |
| **Outline** | Stroke only (3px), transparent fill |

---

## SVG Shape Code

These are the canonical, production-exact SVG paths. Use these paths directly in your HTML/SVG output. The viewBox is `0 0 100 100` for single-shape usage — scale via the `width` and `height` attributes on the `<svg>` element.

### Rounded Square

```svg
<!-- Solid square — replace FILL_COLOR with brand hex -->
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <rect x="2" y="2" width="96" height="96" rx="14" ry="14"
        fill="FILL_COLOR" stroke="FILL_COLOR" stroke-width="3"/>
</svg>

<!-- Outline square -->
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <rect x="2" y="2" width="96" height="96" rx="14" ry="14"
        fill="none" stroke="FILL_COLOR" stroke-width="3"/>
</svg>
```

### Triangle ↗️ (points upper-right — anchor at lower-left)

```svg
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <!-- Solid -->
  <path d="M4 83L82 5l2.5-2.5C89.5 -2.5 98 1 98 8.1V69C98 84.5 85.5 97 69.8 97H8.6C1.5 97 -2 88.4 4 83Z"
        fill="FILL_COLOR" stroke="FILL_COLOR" stroke-width="3" stroke-miterlimit="10"/>
</svg>
```

### Triangle ↙️ (points lower-left — anchor at upper-right)

```svg
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <!-- Solid -->
  <path d="M96 17L18 95l-2.5 2.5C10.5 102.5 2 99 2 91.9V31C2 15.5 14.5 3 30.2 3H91.4C98.5 3 102 11.6 96 17Z"
        fill="FILL_COLOR" stroke="FILL_COLOR" stroke-width="3" stroke-miterlimit="10"/>
</svg>
```

### Triangle ↖️ (points upper-left — anchor at lower-right)

```svg
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <!-- Solid -->
  <path d="M96 83L18 5l-2.5-2.5C10.5 -2.5 2 1 2 8.1V69C2 84.5 14.5 97 30.2 97H91.4C98.5 97 102 88.4 96 83Z"
        fill="FILL_COLOR" stroke="FILL_COLOR" stroke-width="3" stroke-miterlimit="10"/>
</svg>
```

### Triangle ↘️ (points lower-right — anchor at upper-left)

```svg
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <!-- Solid -->
  <path d="M4 17L82 95l2.5 2.5C89.5 102.5 98 99 98 91.9V31C98 15.5 85.5 3 69.8 3H8.6C1.5 3 -2 11.6 4 17Z"
        fill="FILL_COLOR" stroke="FILL_COLOR" stroke-width="3" stroke-miterlimit="10"/>
</svg>
```

### Triangle ⬆️ (points up — anchor at bottom edge)

```svg
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <!-- Solid -->
  <path d="M14 68L50 5l3.5-3.5C57.5 -2.5 65 1 65 8V50C65 65.5 52.5 78 36.8 78H11.6C4.5 78 1 69.4 14 68Z"
        fill="FILL_COLOR" stroke="FILL_COLOR" stroke-width="3" stroke-miterlimit="10"/>
</svg>
```

### Triangle ⬇️ (points down — anchor at top edge)

```svg
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <!-- Solid -->
  <path d="M86 32L50 95l-3.5 3.5C42.5 102.5 35 99 35 92V50C35 34.5 47.5 22 63.2 22H88.4C95.5 22 99 30.6 86 32Z"
        fill="FILL_COLOR" stroke="FILL_COLOR" stroke-width="3" stroke-miterlimit="10"/>
</svg>
```

### Triangle ➡️ (points right — anchor at left edge)

```svg
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <!-- Solid -->
  <path d="M32 14L95 50l3.5 3.5C102.5 57.5 99 65 92 65H50C34.5 65 22 52.5 22 36.8V11.6C22 4.5 30.6 1 32 14Z"
        fill="FILL_COLOR" stroke="FILL_COLOR" stroke-width="3" stroke-miterlimit="10"/>
</svg>
```

### Triangle ⬅️ (points left — anchor at right edge)

```svg
<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <!-- Solid -->
  <path d="M68 86L5 50l-3.5-3.5C-2.5 42.5 1 35 8 35H50C65.5 35 78 47.5 78 63.2V88.4C78 95.5 69.4 99 68 86Z"
        fill="FILL_COLOR" stroke="FILL_COLOR" stroke-width="3" stroke-miterlimit="10"/>
</svg>
```

**Outline variants**: For any shape, set `fill="none"` and keep `stroke="FILL_COLOR" stroke-width="3"`.

---

## Shape Placement Rules

### 1. Corner Anchoring

Shapes always anchor to corners or bleed off edges. They are NEVER placed floating in the middle of a slide.

```
┌────────────────────────┐
│ ↘️ shape               │  ← shape bleeds off upper-left
│                        │
│     [content zone]     │
│                        │
│               ↖️ shape │  ← shape bleeds off lower-right
└────────────────────────┘
```

### 2. Sizing

| Context | Shape Size |
|---------|-----------|
| Large hero accent (slides) | 280–450px wide |
| Medium accent (cards) | 120–200px wide |
| Small decorative detail | 60–100px wide |
| Pattern cluster (many small shapes) | 20–40px each |

### 3. Bleed Percentage

Shapes should bleed off the edge by 30–60% of their size. A 200px shape should show 80–140px and the rest bleeds off.

### 4. Color Pairing Rules

| Background | Shape Color(s) |
|-----------|---------------|
| White / Light | Vitality, Core, Agility, Champion (any solid or outline) |
| Vitality gradient (pink) | Core solid, Agility outline, white outline |
| Agility gradient (blue) | Vitality solid, Core outline, white outline |
| Dark (black/charcoal) | Vitality solid, Agility solid, Champion solid, Mode outline |

### 5. Multi-Shape Composition

Production assets use 2–3 shapes per design:
- **Primary shape**: Large, solid, anchored to a corner — most visual weight
- **Secondary shape**: Medium, different color, opposite corner or adjacent — creates tension
- **Accent detail**: Small outline shape or cluster of small shapes — adds richness

**Example combination (white card):**
- Large Vitality solid ↙️ at lower-right bleeding 50% off
- Small Core outline ↗️ at upper-right bleeding 30% off

**Example combination (blue gradient slide):**
- Large white outline ↗️ upper-right corner
- Small Vitality solid ↙️ lower-right corner

### 6. Pattern Cluster Mode

In the slide shown in Image 2 (stats/donut chart slide), small triangles cluster in a triangular arrangement at the top-right corner:

```
     ▶▶▶▶▶▶
    ▶▶▶▶▶▶
   ▶▶▶▶▶
  ▶▶▶▶
 ▶▶▶
```

This uses 12–18 small (24–32px) ↗️ or ↘️ triangles arranged in a staircase/wedge pattern, fading from larger to smaller. Colors: purple/Core and lighter purple/Core at lower opacity.

---

## CSS Implementation for HTML Assets

```css
.brand-shape {
  position: absolute;
  /* overflow: hidden on parent is required to clip bleeding shapes */
}

.brand-shape--corner-br {
  /* bottom-right anchor, pointing ↙️ */
  bottom: -60px;
  right: -60px;
  width: 200px;
  height: 200px;
}

.brand-shape--corner-tr {
  /* top-right anchor, pointing ↙️ cluster */
  top: 20px;
  right: 20px;
}
```

---

## pptxgenjs Implementation

In PowerPoint via pptxgenjs, shapes are added as SVG images embedded in the slide:

```javascript
// Add a brand triangle shape as SVG
const triangleSvg = `<svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <path d="M4 83L82 5l2.5-2.5C89.5-2.5 98 1 98 8.1V69C98 84.5 85.5 97 69.8 97H8.6C1.5 97-2 88.4 4 83Z"
        fill="#E8236B" stroke="#E8236B" stroke-width="3" stroke-miterlimit="10"/>
</svg>`;

slide.addImage({
  data: 'data:image/svg+xml;base64,' + Buffer.from(triangleSvg).toString('base64'),
  x: 9.5, y: 5.2,    // inches from top-left
  w: 2.5, h: 2.5,    // inches
});
```
