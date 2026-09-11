# ball (units)

board: ui-minigolf-board
projection: isometric
role: npc
style: kenney-pixel-vector
states: { idle: 4, walk: 2 }

The golf ball (0 0 64 64): a white dimpled sphere (#F8FAFC, r 16, centred
(32,34), #1E293B contour stroke) with a bright specular arc on the upper
left, six #CBD5E1 dimples scattered over the lower hemisphere, and a soft
contact shadow ellipse (#0F172A at 25%) under it at (32,50). Drawn for
anchor "center" at 0.35 cell size — it sits on the green, not in the air.

Animation contract: idle is a 4-frame breathing squash/stretch anchored at
the feet (32,50) — never a translate bob; walk is the roll wobble, a ±12°
spin about the ball centre (32,34), shown for ~600ms after each putt before
the tick ages the unit back to idle.

Palette: primary #F8FAFC, secondary #CBD5E1, outline #1E293B.
Geometry: single sphere + contact shadow; frames wrap the same art in a transform.
