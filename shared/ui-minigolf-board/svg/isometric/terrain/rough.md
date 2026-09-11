# rough (terrain)

board: ui-minigolf-board
projection: isometric
role: tile
style: kenney-pixel-vector
states: { static: 1 }

Full-cell isometric cube (0 0 64 64, top diamond 32,16 64,32 32,48 0,32 — the
tessellation contract). The impassable wall block: visibly darker and wilder
than the fairway so the corridor reads at a glance — top face deep green
#2E7D32 with six short grass-blade tuft strokes alternating #4CAF50 and
#1B5E20, side faces #1B5E20 (left) and #14532D (right), contour stroke
#1E293B.

Palette: primary #2E7D32, secondary #1B5E20, outline #1E293B.
Geometry: isometric cube block, full cell; tuft strokes stand up off the top diamond.
