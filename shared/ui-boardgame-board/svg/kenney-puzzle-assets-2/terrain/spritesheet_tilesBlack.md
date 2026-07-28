# Visual Blueprint: spritesheet tilesBlack

- **Asset ID / Stem**: `spritesheet_tilesBlack`
- **Category**: `terrain`
- **Pack Slug**: `kenney-puzzle-assets-2`
- **Board Genre**: `ui-boardgame-board`
- **Target ViewBox**: `0 0 64 64`
- **Projection Type**: `2D Flat Orthographic Sprite (0 0 64 64)`

---

## 1. Object & Silhouette Geometry
Standard rectangular/contour 2D game sprite silhouette with crisp outer border stroke.

## 2. Color Palette & Shading
- **Primary Fill**: `#334155` (CSS token: `fill="var(--color-asset-primary, #334155)"`)
- **Secondary / Side Shading**: `#1E293B` (CSS token: `fill="var(--color-asset-secondary, #1E293B)"`)
- **Deep Shadow Accent**: `#0F172A`
- **Specular Highlight**: `#64748B`
- **Outer Contour Stroke**: `#1E293B` (`stroke-width="2"` or `1.5`)

## 3. Surface Texture & Ornamentation
Smooth surface gradient with clean interior vector highlights and minimal shading.

## 4. XML Group (<g>) Layering Blueprint
When synthesizing the SVG vector code, structure the drawing using these semantic group layers:
1. `<g id="base-shape"> - Outer silhouette background path/rect with border stroke`
2. `<g id="surface-details"> - Interior texture patterns, stripes, and material trim`
3. `<g id="highlights"> - Specular reflection curves and bright top edges`

---

## 5. Subagent Synthesis Prompt
Synthesize a resolution-independent SVG vector graphic for "spritesheet tilesBlack" (spritesheet_tilesBlack) in category "terrain".
Projection: 2D Flat Orthographic Sprite (0 0 64 64).
Shape & Proportions: Standard rectangular/contour 2D game sprite silhouette with crisp outer border stroke.
Surface & Details: Smooth surface gradient with clean interior vector highlights and minimal shading.
Color Scheme: Primary #334155, Secondary #1E293B, Shadow #0F172A, Highlight #64748B, Outline #1E293B.
