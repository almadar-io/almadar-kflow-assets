# Visual Blueprint: hexagonAll sheet

- **Asset ID / Stem**: `hexagonAll_sheet`
- **Category**: `terrain`
- **Pack Slug**: `kenney-hexagon-pack`
- **Board Genre**: `ui-hex-strategy-board`
- **Target ViewBox**: `0 0 64 64`
- **Projection Type**: `6-Sided Hexagonal Grid Tile (0 0 64 64)`

---

## 1. Object & Silhouette Geometry
Regular flat-topped hexagonal polygon silhouette centered at (32,32) with vertices at (32,4), (58,18), (58,46), (32,60), (6,46), (6,18).

## 2. Color Palette & Shading
- **Primary Fill**: `#4CAF50` (CSS token: `fill="var(--color-asset-primary, #4CAF50)"`)
- **Secondary / Side Shading**: `#2E7D32` (CSS token: `fill="var(--color-asset-secondary, #2E7D32)"`)
- **Deep Shadow Accent**: `#1B5E20`
- **Specular Highlight**: `#81C784`
- **Outer Contour Stroke**: `#1E293B` (`stroke-width="2"` or `1.5`)

## 3. Surface Texture & Ornamentation
Hexagonal surface terrain representing hexagonAll sheet with inner border contour lines and themed environmental landmarks.

## 4. XML Group (<g>) Layering Blueprint
When synthesizing the SVG vector code, structure the drawing using these semantic group layers:
1. `<g id="hex-base"> - Outer hexagonal polygon with border stroke #064E3B and primary fill`
2. `<g id="hex-terrain-details"> - Interior terrain symbols, trees, rocks, or water ripples`
3. `<g id="hex-highlight"> - Inner concentric hex outline with 50% opacity highlight`

---

## 5. Subagent Synthesis Prompt
Synthesize a resolution-independent SVG vector graphic for "hexagonAll sheet" (hexagonAll_sheet) in category "terrain".
Projection: 6-Sided Hexagonal Grid Tile (0 0 64 64).
Shape & Proportions: Regular flat-topped hexagonal polygon silhouette centered at (32,32) with vertices at (32,4), (58,18), (58,46), (32,60), (6,46), (6,18).
Surface & Details: Hexagonal surface terrain representing hexagonAll sheet with inner border contour lines and themed environmental landmarks.
Color Scheme: Primary #4CAF50, Secondary #2E7D32, Shadow #1B5E20, Highlight #81C784, Outline #1E293B.
