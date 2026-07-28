# Visual Blueprint: watercraftPack 024 7 sheet

- **Asset ID / Stem**: `watercraftPack_024_7_sheet`
- **Category**: `features`
- **Pack Slug**: `kenney-isometric-watercraft`
- **Board Genre**: `ui-platformer-board`
- **Target ViewBox**: `0 0 64 64`
- **Projection Type**: `3D Axonometric Isometric Cube (0 0 64 64)`

---

## 1. Object & Silhouette Geometry
Isometric cube block with 3 visible diamond/parallelogram faces: top face (points 32,4 58,18 32,32 6,18), left side face (6,18 32,32 32,58 6,44), and right shadow side face (32,32 58,18 58,44 32,58).

## 2. Color Palette & Shading
- **Primary Fill**: `#38BDF8` (CSS token: `fill="var(--color-asset-primary, #38BDF8)"`)
- **Secondary / Side Shading**: `#0284C7` (CSS token: `fill="var(--color-asset-secondary, #0284C7)"`)
- **Deep Shadow Accent**: `#0369A1`
- **Specular Highlight**: `#BAE6FD`
- **Outer Contour Stroke**: `#1E293B` (`stroke-width="2"` or `1.5`)

## 3. Surface Texture & Ornamentation
Translucent aqua blue liquid cube with animated surface wave ripples on top face and caustics on side faces.

## 4. XML Group (<g>) Layering Blueprint
When synthesizing the SVG vector code, structure the drawing using these semantic group layers:
1. `<g id="cube-top-face"> - Top diamond face polygon with primary surface color and top texture`
2. `<g id="cube-left-face"> - Left parallelogram side face polygon with secondary shaded color`
3. `<g id="cube-right-face"> - Right parallelogram side face polygon with dark shadow color`
4. `<g id="face-highlights"> - Crisp white/bright stroke highlights along the top-facing edges`

---

## 5. Subagent Synthesis Prompt
Synthesize a resolution-independent SVG vector graphic for "watercraftPack 024 7 sheet" (watercraftPack_024_7_sheet) in category "features".
Projection: 3D Axonometric Isometric Cube (0 0 64 64).
Shape & Proportions: Isometric cube block with 3 visible diamond/parallelogram faces: top face (points 32,4 58,18 32,32 6,18), left side face (6,18 32,32 32,58 6,44), and right shadow side face (32,32 58,18 58,44 32,58).
Surface & Details: Translucent aqua blue liquid cube with animated surface wave ripples on top face and caustics on side faces.
Color Scheme: Primary #38BDF8, Secondary #0284C7, Shadow #0369A1, Highlight #BAE6FD, Outline #1E293B.
