# Visual Blueprint: groundBeige blue

- **Asset ID / Stem**: `groundBeige_blue`
- **Category**: `terrain`
- **Pack Slug**: `kenney-sports-pack`
- **Board Genre**: `ui-sports-board`
- **Target ViewBox**: `0 0 64 64`
- **Projection Type**: `2D Flat Orthographic Sprite (0 0 64 64)`

---

## 1. Object & Silhouette Geometry
Standard rectangular/contour 2D game sprite silhouette with crisp outer border stroke.

## 2. Color Palette & Shading
- **Primary Fill**: `#38BDF8` (CSS token: `fill="var(--color-asset-primary, #38BDF8)"`)
- **Secondary / Side Shading**: `#0284C7` (CSS token: `fill="var(--color-asset-secondary, #0284C7)"`)
- **Deep Shadow Accent**: `#0369A1`
- **Specular Highlight**: `#BAE6FD`
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
Synthesize a resolution-independent SVG vector graphic for "groundBeige blue" (groundBeige_blue) in category "terrain".
Projection: 2D Flat Orthographic Sprite (0 0 64 64).
Shape & Proportions: Standard rectangular/contour 2D game sprite silhouette with crisp outer border stroke.
Surface & Details: Smooth surface gradient with clean interior vector highlights and minimal shading.
Color Scheme: Primary #38BDF8, Secondary #0284C7, Shadow #0369A1, Highlight #BAE6FD, Outline #1E293B.
