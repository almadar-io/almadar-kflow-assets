# Visual Blueprint: colored packed

- **Asset ID / Stem**: `colored_packed`
- **Category**: `terrain`
- **Pack Slug**: `kenney-1-bit-pack`
- **Board Genre**: `ui-topdown-rts-board`
- **Target ViewBox**: `0 0 64 64`
- **Projection Type**: `2D Flat Orthographic Sprite (0 0 64 64)`

---

## 1. Object & Silhouette Geometry
Standard rectangular/contour 2D game sprite silhouette with crisp outer border stroke.

## 2. Color Palette & Shading
- **Primary Fill**: `#F97316` (CSS token: `fill="var(--color-asset-primary, #F97316)"`)
- **Secondary / Side Shading**: `#EA580C` (CSS token: `fill="var(--color-asset-secondary, #EA580C)"`)
- **Deep Shadow Accent**: `#9A3412`
- **Specular Highlight**: `#FDBA74`
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
Synthesize a resolution-independent SVG vector graphic for "colored packed" (colored_packed) in category "terrain".
Projection: 2D Flat Orthographic Sprite (0 0 64 64).
Shape & Proportions: Standard rectangular/contour 2D game sprite silhouette with crisp outer border stroke.
Surface & Details: Smooth surface gradient with clean interior vector highlights and minimal shading.
Color Scheme: Primary #F97316, Secondary #EA580C, Shadow #9A3412, Highlight #FDBA74, Outline #1E293B.
