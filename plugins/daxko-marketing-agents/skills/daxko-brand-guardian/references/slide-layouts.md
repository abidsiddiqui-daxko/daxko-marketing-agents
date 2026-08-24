> **SOURCE FILE:** `Downloads/daxko-visual-designer 2/references/slide-layouts.md`  ·  **LAST UPDATED:** 2026-03-25 (file date — no "last updated" line stated inside the document)  ·  **Placed in Agent HQ:** 2026-08-11
>
> ✅ **VERIFIED 2026-08-14.** These files did not come from `drop-your-updated-files-here`, but they have been checked byte-for-byte against the `daxko-brand-design-system` skill that is live in Abid Siddiqui's Daxko claude.ai account, and they are IDENTICAL. Confirmed correct by Abid Siddiqui. Full provenance in `visual-brand/INDEX.md`.

# Daxko Slide Layout Patterns

These are the 8 production-proven layout patterns used in Daxko slides and presentations. Every slide should map to one of these layouts or be a deliberate hybrid.

All layouts assume **1920 × 1080px** (or **13.33 × 7.5 in** in PPTX at 144 DPI).

---

## Layout 1: Title / Hero Slide

**Use for:** Opening slide, section dividers, campaign heroes

```
┌──────────────────────────────────────────┐
│ [Logo: top-left, 160px wide]             │
│                                          │
│  ██████████████████                      │
│  HEADLINE                                │
│  ████████                                │
│                                          │
│  Subheadline supporting text here        │
│                                          │
│  [CTA Button]                            │
│                                          │
│                         [Shape ↗️ bleed] │
└──────────────────────────────────────────┘
```

**Specs:**
- Background: Vitality gradient (`linear-gradient(135deg, #B81CB5, #E8236B)`) or Agility gradient
- Logo: White reversed, 160px wide, 40px from top-left corner
- Headline: Barlow SemiBold 600, 60–72pt, white, sentence case
- Subheadline: Sohne Buch 400, 20pt, white
- CTA button: White fill, Vitality 600 text, square corners
- Shape: Large ↗️ triangle solid white, 300–400px, bleeding off lower-right (~40% visible)
- Additional accent: Small outline ↙️ triangle, 80px, upper-right corner

**pptxgenjs positioning:**
```javascript
// Headline
slide.addText(headlineText, {
  x: 0.6, y: 1.8, w: 8, h: 2,
  fontSize: 60, fontFace: 'Barlow', bold: true, color: 'FFFFFF',
});
// CTA
slide.addShape(pptx.ShapeType.rect, {
  x: 0.6, y: 5.0, w: 2.5, h: 0.6,
  fill: { color: 'FFFFFF' }, line: { color: 'FFFFFF' },
});
```

---

## Layout 2: Content + Image (Two-Column)

**Use for:** Feature slides, product benefits, case studies

```
┌──────────────┬───────────────────────────┐
│              │                           │
│  HEADLINE    │  [Photo or illustration   │
│              │   fills entire right half]│
│  Body text   │                           │
│  goes here   │  [optional ↙️ shape       │
│  in this     │   bleeding off corner]    │
│  column      │                           │
│              │                           │
│ [CTA button] │                           │
└──────────────┴───────────────────────────┘
```

**Specs:**
- Left column: 6.5 inches wide, white background
- Right column: 6.83 inches wide, full-bleed photo (`object-fit: cover`)
- Headline: Sohne Halbfett 600, 36–44pt, `#000000` (or white if dark BG)
- Body: Sohne Buch 400, 16pt, `#595959`
- Photo accent shape: Medium ↙️ triangle 150px, bleeding off photo corner
- Logo: Bottom-left, 120px wide

**Curved divider variant** (Image 3 — Email Banner):
Replace the straight column edge with a large curved white mask that sweeps from upper-left to lower-right, creating an organic split between text and photo sides. The curve radius is roughly 15–20% of the slide width.

---

## Layout 3: Stats / Data Visualization

**Use for:** Results slides, metrics, benchmark comparisons

```
┌──────────────────────────────────────────┐
│ HEADLINE                   [shape cluster│
│ Subtitle as needed          top-right ↗️]│
│                                          │
│  ┌────────┐  ┌────────┐  ┌────────┐     │
│  │ DONUT  │  │ DONUT  │  │ DONUT  │     │
│  │  85%   │  │  90%   │  │  105%  │     │
│  └────────┘  └────────┘  └────────┘     │
│  Time-savings  Cheaper ads  CTR          │
│                                          │
│              [ CTA BUTTON ]              │
│ [Logo]            [copyright]            │
└──────────────────────────────────────────┘
```

**Specs:**
- Background: White
- Headline: Sohne Halbfett 600, 40pt, `#595959` (medium gray)
- Subtitle: Sohne Buch 400, 18pt, `#595959`
- Stat label: Sohne Halbfett 600, 18pt, `#595959`
- Stat value inside donut: Sohne Halbfett 600, 52pt, matching donut color
- Donut chart colors: Agility 500 `#038BED`, Champion 300 `#FBB03B`, Core 700 `#B81CB5`
- Inactive donut track: `#E0E0E0`
- CTA button: Vitality gradient fill, white text, square corners, 180×50px
- **Top-right corner**: Shape cluster (see `brand-patterns.md` → Pattern Cluster Mode)
- Logo: Bottom-left, full-color, 60px wide
- Copyright line: `© 2025 Daxko`, 10pt, `#595959`

**Donut chart HTML:**
```html
<div style="
  width: 220px; height: 220px; border-radius: 50%;
  background: conic-gradient(#038BED 0% 85%, #E0E0E0 85% 100%);
  display: flex; align-items: center; justify-content: center;
  position: relative;
">
  <div style="
    width: 160px; height: 160px; border-radius: 50%;
    background: white;
    display: flex; align-items: center; justify-content: center;
    font: 600 52px 'Sohne', sans-serif; color: #038BED;
  ">85%</div>
</div>
```

---

## Layout 4: Full-Bleed Photo + Text Overlay

**Use for:** Hero slides, emotional campaigns, customer stories

```
┌──────────────────────────────────────────┐
│ [Full slide photo, darkened 40% overlay] │
│                                          │
│  [Logo top-left white]                   │
│                                          │
│                                          │
│  HEADLINE IN WHITE                       │
│  Subhead text in white                   │
│                                          │
│  [CTA button]                            │
│                                          │
│    [↗️ white outline shape, lower-right] │
└──────────────────────────────────────────┘
```

**Specs:**
- Photo: full coverage, `object-fit: cover`
- Overlay: `rgba(0,0,0,0.45)` or brand color at 50–60% opacity
- All text: White
- Shape: White outline ↗️, 250px, lower-right corner bleeding 50%

---

## Layout 5: Portrait Card (Vertical Format)

**Use for:** Social media cards, digital ads, direct mail pieces (Image 1 style)

```
┌─────────────────────────┐
│ [Product logo top-left] │
│                         │
│  HEADLINE IS            │
│  PLACED HERE            │
│  LIKE THIS              │
│                         │
│  Subhead follows        │
│  as a short blurb       │
│                         │
│           [Person photo │
│            bleeding out │
│            of the card] │
│    [Shape ↙️/↖️ corner] │
└─────────────────────────┘
```

**Specs (1000 × 1400px):**
- Background options: White (top cards), Vitality/Agility/Core/Champion gradient (bottom cards)
- Product logo: top-left, 140px wide, 40px margin
- Headline: Sohne Halbfett 600, 44–52pt
  - On white bg: `#000000`
  - On colored bg: `#FFFFFF`
- Subhead: Sohne Buch 400, 18pt, same color rule as headline
- Photo: Isolated/cutout photography of a person, positioned right-center, bleeds off right and top edges
- Shape accent: 1–2 brand shapes, 100–180px, in brand colors, anchored to corners opposite the photo
- CTA button: Optional, bottom-left area

**Background color rules for portrait cards:**
- White background: shapes in any brand color
- Pink/Vitality gradient: shapes in Core (purple) or Agility (blue)
- Blue/Agility gradient: shapes in Vitality (pink) or Core (purple)
- Orange gradient: shapes in Core (purple) or Vitality (pink)
- Purple/Core gradient: shapes in Agility (blue) or Vitality (pink)

---

## Layout 6: Icon + Feature Grid

**Use for:** Product feature lists, benefit comparisons, service overviews

```
┌──────────────────────────────────────────┐
│  HEADLINE                                │
│  Subtitle                                │
│  ──────────────────────────────────────  │
│  [Icon] Feature name    [Icon] Feature   │
│         Description           Descript.  │
│                                          │
│  [Icon] Feature name    [Icon] Feature   │
│         Description           Descript.  │
│                                          │
│  [Icon] Feature name    [Icon] Feature   │
│         Description           Descript.  │
│  ──────────────────────────────────────  │
│  [Logo]                    [CTA button]  │
└──────────────────────────────────────────┘
```

**Specs:**
- Background: White or `#F6F6F6`
- Headline: Sohne Halbfett 600, 36pt, `#000000`
- Icon: Colored brand shape (20–30px) OR monochrome icon in brand color circle
- Feature name: Sohne Halbfett 600, 16pt, `#000000`
- Description: Sohne Buch 400, 13pt, `#595959`
- Column divider: `#E0E0E0` 1px line (optional)
- CTA: Vitality 600 fill, white text

---

## Layout 7: Big Quote / Testimonial

**Use for:** Customer testimonials, key messages, pull quotes

```
┌──────────────────────────────────────────┐
│ [gradient BG or dark BG]                 │
│                                          │
│    ❝                                     │
│    BIG QUOTE TEXT GOES                   │
│    HERE ACROSS 2–3 LINES                 │
│                                          │
│    — Customer Name, Title                │
│      Company                             │
│                                          │
│ [↙️ shape lower-right]  [Logo]          │
└──────────────────────────────────────────┘
```

**Specs:**
- Background: Core gradient or dark `#1A1A1A`
- Quote mark: Vitality 600, Barlow 600, 120pt
- Quote text: Sohne Buch 400 or Barlow 600, 28–36pt, white
- Attribution: Sohne Buch 400, 14pt, `rgba(255,255,255,0.7)`
- Shape: Vitality or Agility solid, ↙️, 200px, lower-right

---

## Layout 8: Agenda / Section Header

**Use for:** Agenda slides, section transitions

```
┌──────────────────────────────────────────┐
│ [colored left bar, 8px wide]             │
│                                          │
│  01  Section or agenda item title        │
│      Brief descriptor                    │
│  ────────────────────────────────        │
│  02  Section or agenda item title        │
│      Brief descriptor                    │
│  ────────────────────────────────        │
│  03  Section or agenda item title        │
│      Brief descriptor                    │
│                                          │
│ [Logo]                                   │
└──────────────────────────────────────────┘
```

**Specs:**
- Background: White
- Left bar: 8px wide, Vitality 600 or brand gradient
- Number: Sohne Halbfett 600, 48pt, Vitality 600 or Core 700
- Title: Sohne Halbfett 600, 22pt, `#000000`
- Descriptor: Sohne Buch 400, 14pt, `#595959`
- Divider: `#E0E0E0`, 1px

---

## Slide Footer Standard

All slides except full-bleed hero should include:

```
[Logo left]          [Slide content]          [Page number right]
                  © 2025 Daxko
```

- Footer y position: 7.1–7.4 inches from top (near bottom of 7.5in slide)
- Logo: 80px wide, full-color on white slides, white reversed on dark slides
- Copyright: Sohne Buch 400, 10pt, `#595959` or white

---

## Slide Background Color Mapping

| Slide Purpose | Background |
|--------------|-----------|
| Title / Hero | Brand gradient or Agility gradient |
| Content / Data | White `#FFFFFF` |
| Testimonial | Core gradient or `#1A1A1A` |
| Section header | White or `#F6F6F6` |
| Closing / CTA | Vitality gradient |

---

## pptxgenjs Master Dimensions

```javascript
const pptx = new PptxGenJS();
pptx.layout = 'LAYOUT_WIDE';  // 13.33 x 7.5 inches
// Colors in hex without '#'
// Positions in inches from top-left
// Font 'Barlow' for display, 'Calibri' as system fallback for Sohne
```
