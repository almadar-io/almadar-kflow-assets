# fairway (terrain)

board: ui-minigolf-board
projection: isometric
role: tile
style: kenney-pixel-vector
states: { static: 1 }

Full-cell isometric cube (0 0 64 64, top diamond 32,16 64,32 32,48 0,32 — the
tessellation contract: side faces run to the bottom edge so adjacent cubes
render connected with no gaps). The mown putting surface: top face primary
green #4CAF50 with an alternating lighter mown-stripe inset diamond #66BB6A
(55% opacity) and a core diamond back at primary, side faces #2E7D32 (left)
and #1B5E20 (right), contour stroke #1E293B.

Palette: primary #4CAF50, secondary #2E7D32, outline #1E293B.
Geometry: isometric cube block, full cell; stripe detail lives on the top diamond only.
