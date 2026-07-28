# Visual Blueprint: foliagePack retina

- **Asset ID / Stem**: `foliagePack_retina`
- **Category**: `features`
- **Pack Slug**: `kenney-foliage-pack`
- **Board Genre**: `ui-fishing-board`
- **Target ViewBox**: `0 0 64 64`
- **Projection Type**: `2D Flat Orthographic Sprite (0 0 64 64)`

---

## 1. Object & Silhouette Geometry
Standard rectangular/contour 2D game sprite silhouette with crisp outer border stroke.

## 2. Color Palette & Shading
- **Primary Fill**: `#4CAF50` (CSS token: `fill="var(--color-asset-primary, #4CAF50)"`)
- **Secondary / Side Shading**: `#2E7D32` (CSS token: `fill="var(--color-asset-secondary, #2E7D32)"`)
- **Deep Shadow Accent**: `#1B5E20`
- **Specular Highlight**: `#81C784`
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
Synthesize a resolution-independent SVG vector graphic for "foliagePack retina" (foliagePack_retina) in category "features".
Projection: 2D Flat Orthographic Sprite (0 0 64 64).
Shape & Proportions: Standard rectangular/contour 2D game sprite silhouette with crisp outer border stroke.
Surface & Details: Smooth surface gradient with clean interior vector highlights and minimal shading.
Color Scheme: Primary #4CAF50, Secondary #2E7D32, Shadow #1B5E20, Highlight #81C784, Outline #1E293B.
