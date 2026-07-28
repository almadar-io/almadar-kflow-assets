# Visual Blueprint: cardsLarge tilemap packed

- **Asset ID / Stem**: `cardsLarge_tilemap_packed`
- **Category**: `terrain`
- **Pack Slug**: `kenney-playing-cards-pack`
- **Board Genre**: `ui-boardgame-board`
- **Target ViewBox**: `0 0 512 716`
- **Projection Type**: `Playing Card Face Vector (0 0 512 716)`

---

## 1. Object & Silhouette Geometry
Vertical playing card rectangle (480x684px) centered with rounded 24px corners and inner decorative card border.

## 2. Color Palette & Shading
- **Primary Fill**: `#1E293B` (CSS token: `fill="var(--color-asset-primary, #1E293B)"`)
- **Secondary / Side Shading**: `#0F172A` (CSS token: `fill="var(--color-asset-secondary, #0F172A)"`)
- **Deep Shadow Accent**: `#1B5E20`
- **Specular Highlight**: `#81C784`
- **Outer Contour Stroke**: `#1E293B` (`stroke-width="2"` or `1.5`)

## 3. Surface Texture & Ornamentation
Card rank "CAR" displayed in top-left and bottom-right corners with large central suit emblem symbol for cardsLarge tilemap packed.

## 4. XML Group (<g>) Layering Blueprint
When synthesizing the SVG vector code, structure the drawing using these semantic group layers:
1. `<g id="card-background"> - White card background rect with bold dark border stroke`
2. `<g id="card-inner-frame"> - Dashed/decorative inner border frame rectangle`
3. `<g id="card-corner-ranks"> - Top-left and inverted bottom-right rank text and mini suit emblems`
4. `<g id="card-center-emblem"> - Large central suit emblem graphic vector shape`

---

## 5. Subagent Synthesis Prompt
Synthesize a resolution-independent SVG vector graphic for "cardsLarge tilemap packed" (cardsLarge_tilemap_packed) in category "terrain".
Projection: Playing Card Face Vector (0 0 512 716).
Shape & Proportions: Vertical playing card rectangle (480x684px) centered with rounded 24px corners and inner decorative card border.
Surface & Details: Card rank "CAR" displayed in top-left and bottom-right corners with large central suit emblem symbol for cardsLarge tilemap packed.
Color Scheme: Primary #1E293B, Secondary #0F172A, Shadow #1B5E20, Highlight #81C784, Outline #1E293B.
