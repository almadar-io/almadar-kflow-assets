# Visual Blueprint: genericItems spritesheet white

- **Asset ID / Stem**: `genericItems_spritesheet_white`
- **Category**: `features`
- **Pack Slug**: `kenney-generic-items`
- **Board Genre**: `ui-city-builder-board`
- **Target ViewBox**: `0 0 64 64`
- **Projection Type**: `2D Flat Orthographic Sprite (0 0 64 64)`

---

## 1. Object & Silhouette Geometry
Standard rectangular/contour 2D game sprite silhouette with crisp outer border stroke.

## 2. Color Palette & Shading
- **Primary Fill**: `#F8FAFC` (CSS token: `fill="var(--color-asset-primary, #F8FAFC)"`)
- **Secondary / Side Shading**: `#E2E8F0` (CSS token: `fill="var(--color-asset-secondary, #E2E8F0)"`)
- **Deep Shadow Accent**: `#94A3B8`
- **Specular Highlight**: `#FFFFFF`
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
Synthesize a resolution-independent SVG vector graphic for "genericItems spritesheet white" (genericItems_spritesheet_white) in category "features".
Projection: 2D Flat Orthographic Sprite (0 0 64 64).
Shape & Proportions: Standard rectangular/contour 2D game sprite silhouette with crisp outer border stroke.
Surface & Details: Smooth surface gradient with clean interior vector highlights and minimal shading.
Color Scheme: Primary #F8FAFC, Secondary #E2E8F0, Shadow #94A3B8, Highlight #FFFFFF, Outline #1E293B.
