> **SOURCE FILE:** `Downloads/daxko-visual-designer 2/references/photography-layout.md`  ·  **LAST UPDATED:** 2026-03-25 (file date — no "last updated" line stated inside the document)  ·  **Placed in Agent HQ:** 2026-08-11
>
> ✅ **VERIFIED 2026-08-14.** These files did not come from `drop-your-updated-files-here`, but they have been checked byte-for-byte against the `daxko-brand-design-system` skill that is live in Abid Siddiqui's Daxko claude.ai account, and they are IDENTICAL. Confirmed correct by Abid Siddiqui. Full provenance in `visual-brand/INDEX.md`.

# Daxko Photography Layout Guide

Daxko brand photography should feel energetic, human, and authentic. Photography is always combined with brand elements — shapes, colors, and layout structure — in specific, intentional ways.

---

## Photography Style

### Subject Guidelines

- **People-forward**: Primary subject is always a person engaged in fitness, health, or wellness activity
- **Authentic moments**: Natural, in-action shots — not posed stock photography
- **Diverse representation**: Mix of ages, genders, ethnicities, and fitness levels
- **Technology integration**: Subjects often shown with phones, tablets, or check-in screens (product context)

### Subject Types in Production

| Subject | Context |
|---------|---------|
| Youth athlete | Youth sports programs (Operations branding) |
| Adult fitness member | Gym/club engagement (Club Automation, Zen Planner) |
| Martial arts student | Zen Planner |
| Senior wellness | YMCA/community center (Operations) |
| Front desk/staff | Check-in, onboarding, customer service |

### Isolated Photography ("Cutout" Style)

The most common Daxko photography style: the subject is photographed against a white or solid background, creating a clean cutout look where the person appears to float on or bleed off the edge of the design.

**Rules for isolated photography:**
- Subject is cropped cleanly — no visible background behind them
- Subject bleeds off at least one edge of the design (usually right or top)
- Subject appears in front of all design elements
- `z-index` of photo is higher than background colors and shapes
- Background of the card/slide shows through around the subject

**CSS implementation:**
```css
.photo-isolated {
  position: absolute;
  bottom: 0;
  right: -20px;        /* slight bleed off right edge */
  height: 85%;         /* occupies most of the card height */
  object-fit: contain; /* preserve aspect ratio, no crop */
  z-index: 3;          /* above shapes and background */
}
```

---

## Photo Layout Patterns

### 1. Portrait Card — Right Bleed

Used in Image 1 (DM_Example_Isolated_photography). The person stands in the right half of the card, bleeding off the right and sometimes top edge.

```
┌─────────────────────────┐
│ [Logo top-left]         │
│                         │
│  Headline               │  ← z-index: 2
│  text here              │
│               [PERSON   │  ← z-index: 3 (above headline bg)
│               bleeding  │
│  Subhead text  right ↑] │
│                         │
│ [Shape ↙️]              │  ← z-index: 1 (behind text)
└─────────────────────────┘
```

**Proportions:**
- Text content: Left 55–60% of card width
- Photo: Right 70–80% of card width (overlapping text area with transparency)
- Shape: Opposite corner from photo (lower-left or upper-left)

### 2. Wide Banner — Right Panel

Used in Image 3 (Email_Photo_in_triangle_on_light). The banner splits into a white content panel (left 60%) and a photo panel (right 40%). A large curved white mask divides them.

```
┌──────────────────────┬─────────────────┐
│ [Logo]               │                 │
│                      │   [Full photo   │
│  Big headline        │    no cutout,   │
│  goes here           │    object-fit:  │
│                      │    cover]       │
│  Subhead text        │                 │
└──────────────────────┴─────────────────┘
```

**Curved mask implementation (the distinctive arc divider):**
```css
.photo-panel {
  position: absolute;
  top: 0; right: 0;
  width: 45%;
  height: 100%;
  overflow: hidden;
}

.photo-panel::before {
  content: '';
  position: absolute;
  top: -10%;
  left: -15%;
  width: 35%;
  height: 120%;
  background: white;  /* same as banner background */
  border-radius: 0 60% 60% 0 / 0 50% 50% 0;
  z-index: 2;
}

.photo-panel img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

**Pattern overlay on white panel:**
The white panel area (not the photo) uses the Small Grid Light pattern at 10–12% opacity as background texture.

### 3. Slide — Half-Bleed (Two-Column with Photo Right)

The right half of the slide is a full-bleed photo. The left half is a white or gradient content area.

```javascript
// pptxgenjs implementation
slide.addImage({
  path: 'photo.jpg',
  x: 6.67, y: 0,    // right half
  w: 6.66, h: 7.5,
  sizing: { type: 'cover', w: 6.66, h: 7.5 }
});
```

### 4. Triangle Photo Frame

A distinctive Daxko treatment: the photo is masked inside a large triangle shape, creating a geometric window effect. The triangle points toward a corner of the slide.

```css
.photo-triangle-frame {
  clip-path: polygon(0 100%, 100% 0, 100% 100%);  /* ↗️ triangle */
  /* adjust polygon points for other orientations */
}
```

**Common orientations:**
- ↙️ (lower-left triangle frame): `clip-path: polygon(0 0, 100% 0, 0 100%)`
- ↗️ (upper-right triangle frame): `clip-path: polygon(0 100%, 100% 0, 100% 100%)`
- ↘️: `clip-path: polygon(100% 0, 0 0, 100% 100%)`

---

## Color Overlays on Photography

When placing photos on colored backgrounds, add a semi-transparent color overlay to blend the photo with the design:

| Background | Overlay Color | Overlay Opacity |
|-----------|--------------|----------------|
| Vitality gradient (pink) | `#E8236B` | 40–50% |
| Agility gradient (blue) | `#038BED` | 40–50% |
| Core gradient (purple) | `#B81CB5` | 40–50% |
| White | None | — |
| Dark/black | `#000000` | 30–40% |

**CSS implementation:**
```css
.photo-with-overlay {
  position: relative;
}
.photo-with-overlay::after {
  content: '';
  position: absolute;
  inset: 0;
  background: rgba(184, 28, 181, 0.45); /* Core 700 at 45% */
  mix-blend-mode: multiply;
}
```

---

## Photography + Shape Layering

The correct z-index stack for a portrait card:

```
z-index: 4  │ Text / headline (foreground)
z-index: 3  │ Isolated photo (person)
z-index: 2  │ Brand shapes (decorative)
z-index: 1  │ Background color / gradient
z-index: 0  │ Pattern overlay
```

**Key rule**: The person is always visually "in front of" brand shapes, but "behind" text content so the headline is always readable.

---

## Aspect Ratios for Common Photo Slots

| Context | Aspect Ratio | Note |
|---------|-------------|------|
| Portrait card, right panel | 3:4 | Portrait orientation |
| Slide, right half | 1:1 to 16:9 | Depends on slide |
| Email banner, right panel | 1:1.2 | Slightly tall |
| Wide social post, right | 1:1 | Square |
| Square social post | Fill | Object-fit: cover |

---

## Photography Checklist

Before finalizing any asset with photography:

- [ ] Photo subject is clearly visible and not clipped awkwardly
- [ ] Isolated photo bleeds off at least one edge (portrait card style)
- [ ] Photo is on the correct z-index layer (above shapes, below text)
- [ ] Text is readable against the photo (sufficient contrast)
- [ ] If photo is on a colored background, color overlay is applied
- [ ] Photo aspect ratio matches the container dimensions
