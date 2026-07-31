# crew (units)

board: ui-space-station-board
projection: isometric
role: npc
style: kenney-pixel-vector
states: { idle: 4, walk: 2, attack: 1, hit: 1, death: 1 }

Synthesize a resolution-independent SVG vector graphic for "crew" (crew) in category "units".
Projection: 3D Axonometric Isometric Cube (0 0 64 64).
Shape & Proportions: A single station crew member in a sky-blue pressure suit with a dark collar ring, reading clearly at one isometric tile; soft contact shadow grounds the feet.
Surface & Details: Friendly face visor with eyes and smile so the unit reads as a person, not a machine; idle is a 4-frame breathing squash/stretch anchored at the feet (never a vertical translate bob); walk is a 2-frame limb-offset cycle; attack/hit/death single frames complete the actor contract (this non-combat board plays idle/walk only).
Color Scheme: Primary #38BDF8, Secondary #0284C7, Shadow #075985, Highlight #BAE6FD, Outline #1E293B.

Palette: primary #38BDF8, secondary #075985, outline #1E293B.
Geometry: Isometric cube block with 3 visible diamond/parallelogram faces: top face (points 32,4 58,18 32,32 6,18), left side face (6,18 32,32 32,58 6,44), and right shadow side face (32,32 58,18 58,44 32,58).
