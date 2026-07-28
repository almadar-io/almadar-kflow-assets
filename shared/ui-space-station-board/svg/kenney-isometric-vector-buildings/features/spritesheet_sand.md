# Visual Blueprint: spritesheet sand

- **Asset ID / Stem**: `spritesheet_sand`
- **Category**: `features`
- **Pack Slug**: `kenney-isometric-vector-buildings`
- **Board Genre**: `ui-space-station-board`
- **Target ViewBox**: `0 0 64 64`
- **Projection Type**: `3D Axonometric Isometric Cube (0 0 64 64)`

---

## 1. Object & Silhouette Geometry
Isometric cube block with 3 visible diamond/parallelogram faces: top face (points 32,4 58,18 32,32 6,18), left side face (6,18 32,32 32,58 6,44), and right shadow side face (32,32 58,18 58,44 32,58).

## 2. Color Palette & Shading
- **Primary Fill**: `#FDE047` (CSS token: `fill="var(--color-asset-primary, #FDE047)"`)
- **Secondary / Side Shading**: `#EAB308` (CSS token: `fill="var(--color-asset-secondary, #EAB308)"`)
- **Deep Shadow Accent**: `#CA8A04`
- **Specular Highlight**: `#FEF08A`
- **Outer Contour Stroke**: `#1E293B` (`stroke-width="2"` or `1.5`)

## 3. Surface Texture & Ornamentation
Clean isometric block faces with directional lighting: brightest on top diamond, medium on left parallelogram, shadow on right parallelogram.

## 4. XML Group (<g>) Layering Blueprint
When synthesizing the SVG vector code, structure the drawing using these semantic group layers:
1. `<g id="cube-top-face"> - Top diamond face polygon with primary surface color and top texture`
2. `<g id="cube-left-face"> - Left parallelogram side face polygon with secondary shaded color`
3. `<g id="cube-right-face"> - Right parallelogram side face polygon with dark shadow color`
4. `<g id="face-highlights"> - Crisp white/bright stroke highlights along the top-facing edges`

---

## 5. Subagent Synthesis Prompt
Synthesize a resolution-independent SVG vector graphic for "spritesheet sand" (spritesheet_sand) in category "features".
Projection: 3D Axonometric Isometric Cube (0 0 64 64).
Shape & Proportions: Isometric cube block with 3 visible diamond/parallelogram faces: top face (points 32,4 58,18 32,32 6,18), left side face (6,18 32,32 32,58 6,44), and right shadow side face (32,32 58,18 58,44 32,58).
Surface & Details: Clean isometric block faces with directional lighting: brightest on top diamond, medium on left parallelogram, shadow on right parallelogram.
Color Scheme: Primary #FDE047, Secondary #EAB308, Shadow #CA8A04, Highlight #FEF08A, Outline #1E293B.
