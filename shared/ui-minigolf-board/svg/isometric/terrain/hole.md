# hole (terrain)

board: ui-minigolf-board
projection: isometric
role: tile
style: kenney-pixel-vector
states: { static: 1 }

Full-cell isometric cube (0 0 64 64, top diamond 32,16 64,32 32,48 0,32 — the
tessellation contract). The cup — the target every putt hunts: mown fairway
green top face (#4CAF50 with the #66BB6A mown-stripe inset, sides #2E7D32 /
#1B5E20) with a dark open cup ellipse (#0F172A, rx 7, ry 3.5) sunk at (32,36)
on the diamond, a white flagstick (#E2E8F0 pole) rising from the cup to y 10,
and a red pennant (#EF4444, #1E293B outline) flying at the top so the hole
reads from across the course.

Palette: primary #4CAF50, secondary #2E7D32, outline #1E293B.
Geometry: isometric cube block, full cell; cup ellipse at (32,36), flagstick + pennant above.
