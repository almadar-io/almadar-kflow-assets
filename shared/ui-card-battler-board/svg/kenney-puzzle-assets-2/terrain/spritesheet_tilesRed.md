# Visual Blueprint: spritesheet tilesRed

- **Asset ID / Stem**: `spritesheet_tilesRed`
- **Category**: `terrain`
- **Pack Slug**: `kenney-puzzle-assets-2`
- **Board Genre**: `ui-card-battler-board`
- **Target ViewBox**: `0 0 512 716`
- **Projection Type**: `Playing Card Face Vector (0 0 512 716)`

---

## 1. Object & Silhouette Geometry
Vertical playing card rectangle (480x684px) centered with rounded 24px corners and inner decorative card border.

## 2. Color Palette & Shading
- **Primary Fill**: `#EF4444` (CSS token: `fill="var(--color-asset-primary, #EF4444)"`)
- **Secondary / Side Shading**: `#DC2626` (CSS token: `fill="var(--color-asset-secondary, #DC2626)"`)
- **Deep Shadow Accent**: `#9A3412`
- **Specular Highlight**: `#FDBA74`
- **Outer Contour Stroke**: `#1E293B` (`stroke-width="2"` or `1.5`)

## 3. Surface Texture & Ornamentation
Card rank "SPR" displayed in top-left and bottom-right corners with large central suit emblem symbol for spritesheet tilesRed.

## 4. XML Group (<g>) Layering Blueprint
When synthesizing the SVG vector code, structure the drawing using these semantic group layers:
1. `<g id="card-background"> - White card background rect with bold dark border stroke`
2. `<g id="card-inner-frame"> - Dashed/decorative inner border frame rectangle`
3. `<g id="card-corner-ranks"> - Top-left and inverted bottom-right rank text and mini suit emblems`
4. `<g id="card-center-emblem"> - Large central suit emblem graphic vector shape`

---

## 5. Subagent Synthesis Prompt
Synthesize a resolution-independent SVG vector graphic for "spritesheet tilesRed" (spritesheet_tilesRed) in category "terrain".
Projection: Playing Card Face Vector (0 0 512 716).
Shape & Proportions: Vertical playing card rectangle (480x684px) centered with rounded 24px corners and inner decorative card border.
Surface & Details: Card rank "SPR" displayed in top-left and bottom-right corners with large central suit emblem symbol for spritesheet tilesRed.
Color Scheme: Primary #EF4444, Secondary #DC2626, Shadow #9A3412, Highlight #FDBA74, Outline #1E293B.
