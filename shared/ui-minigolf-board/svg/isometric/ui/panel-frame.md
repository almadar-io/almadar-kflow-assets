# panel-frame (ui)

board: ui-minigolf-board
projection: isometric
role: ui
style: kenney-pixel-vector
states: { static: 1 }

Cream clubhouse panel (0 0 64 64): rounded #F5F0E1 plate with a #8D7B5E
contour stroke and an inner #D8CDB4 frame line — the shared chrome style
preset every migrated board carries, used for the game-shell background and
the HUD background (wired url-only; the AtlasPanel slice is a known
substrate no-op for url-only svg, gap already recorded).

Palette: primary #F5F0E1, secondary #D8CDB4, outline #8D7B5E.
Geometry: rounded rect plate + inner frame rect.
