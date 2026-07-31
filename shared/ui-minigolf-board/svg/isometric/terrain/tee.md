# tee (terrain)

board: ui-minigolf-board
projection: isometric
role: tile
style: kenney-pixel-vector
states: { static: 1 }

Full-cell isometric cube (0 0 64 64, top diamond 32,16 64,32 32,48 0,32 — the
tessellation contract). The tee box: the same mown fairway green (#4CAF50
with the #66BB6A mown-stripe inset, sides #2E7D32 / #1B5E20) carrying a
white tee-ground marker at the diamond centre — a #F8FAFC ellipse (rx 8,
ry 4) with #1E293B stroke and a #CBD5E1 inner ellipse, the spot the ball
starts from.

Palette: primary #4CAF50, secondary #2E7D32, outline #1E293B.
Geometry: isometric cube block, full cell; tee marker centred at (32,32) on the top diamond.
