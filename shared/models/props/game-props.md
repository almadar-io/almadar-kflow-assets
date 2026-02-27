# Game Props — Collectibles & Story Items

> 5 key interactive props for the Iram Dominion. These are small-to-medium objects the player encounters during gameplay: collectibles, story items, loot containers, and UI markers.

## Art Style Reference

All props follow the Iram Dominion aesthetic: industrial sci-fi with mystical energy. Dark steel and copper metals, teal-cyan resonance energy, red compliance energy. Surfaces are worn, riveted, and industrial — never clean or pristine. Energy effects (glow cores, wisps, pulses) are handled in-engine; the mesh should include the geometry that emits light but the glow itself is a shader effect.

---

## 1. Orbital Shard

### Game Purpose

The primary collectible in Iram. Orbital Shards are crystalline fragments of resonance energy scattered throughout every zone. Collecting them unlocks and upgrades the player's Orbital abilities. Different orbital types have different colors (Disrupt = teal, Defend = gold, Mend = green, etc.), but all share the same base mesh — color variation is applied in code via shader tinting. This prompt generates the teal base version.

### Meshy AI Prompt

```
A small floating crystalline shard for a 3D action RPG. Sci-fi fantasy collectible item.

The shard is an octahedral crystal shape — two four-sided pyramids joined at the base, forming an eight-faced diamond. The crystal has sharp, clean facets with slightly beveled edges. The surface material is translucent teal-cyan crystal with a bright glowing core visible inside, like energy trapped within glass. Small geometric facets catch light at different angles.

The crystal sits on a very thin dark steel ring at its equator — a minimal metal band with tiny etched circuit-line patterns, suggesting it was once part of a larger device. Two or three tiny crystalline splinter fragments float nearby, broken off from the main shard, orbiting loosely.

The overall shape is tall and narrow — taller than it is wide, like a elongated diamond. The color is entirely teal-cyan crystal with the dark steel equator band as the only metal element. The core glow is brighter teal-white at the center, fading to deeper teal at the facet edges.

No base or pedestal. The object floats freely. Low-poly game-ready style with clean geometry. Stylized, not photorealistic.
```

### Output

- **Format:** GLB (static mesh)
- **Save to:** `projects/iram/assets/models/props/orbital-shard.glb`
- **Dimensions:** ~0.3 x 0.3 x 0.5 units (small pickup item)
- **Poly budget:** 200-500 tris
- **Texture:** 256x256 PBR (albedo + emissive for glow core)
- **Animation:** None baked — floating bob and rotation are driven by code (simple sine wave Y-offset + constant Y-axis rotation). Energy particle wisps are a runtime particle system attached to the object.

---

## 2. Resonance Crystal (Large)

### Game Purpose

The story MacGuffin. This is the ancient crystalline formation that Unit 734 discovers deep in the mines beneath Raqim — the "Teacher's Resonance" that cracks his Compliance Engine and awakens Orbital Resonance within him. It appears in the opening cinematic, in several story cutscenes, and as a large interactable object in the first dungeon. Much larger and more dramatic than orbital shards. It looks ancient, alien, and powerful — something that has been growing in the deep rock for millennia.

### Meshy AI Prompt

```
A large ancient crystal cluster growing from a rough rock base, for a 3D action RPG. Alien artifact buried deep underground in an industrial sci-fi setting.

The base is a chunk of rough, dark grey-brown rock — jagged and uneven, as if broken from a cave wall. From the rock, a cluster of five or six large crystalline spires grow upward at slightly different angles, like a crystal formation. The largest central spire is the tallest, with smaller crystals flanking it.

The crystals are translucent teal-cyan with a brilliant bright teal-white core that illuminates the surrounding rock. The crystal surfaces have sharp geometric facets, but the edges show signs of immense age — tiny chips, hairline fractures, and faint etched markings on the largest facets. The etchings resemble alien script or circuit diagrams — geometric lines and dots that are clearly artificial, not natural crystal patterns.

Thin veins of teal energy run through the rock base, branching outward from where the crystals meet the stone, as if the crystal's power is bleeding into the surrounding geology. Small crystal fragments are partially embedded in the rock around the base.

The overall impression is "ancient alien technology disguised as geology." The crystals are clearly not natural mineral formations — they are too geometric, too bright, and the etched script proves intelligent origin. Color palette: dark grey-brown rock base, teal-cyan crystals, bright teal-white core glow, faint teal veins in rock.

Low-poly game-ready style. Stylized, not photorealistic. The rock base should sit flat on a surface.
```

### Output

- **Format:** GLB (static mesh)
- **Save to:** `projects/iram/assets/models/props/resonance-crystal.glb`
- **Dimensions:** ~1.0 x 1.0 x 2.0 units (medium set piece, roughly chest-to-head height on Unit 734)
- **Poly budget:** 1,000-2,000 tris
- **Texture:** 512x512 PBR (albedo + normal for rock detail + emissive for crystal glow and vein glow)
- **Animation:** None baked — ambient pulsing glow is driven by an emissive shader animation in code (slow sine pulse on emissive intensity). Particle motes rising from crystal tips are a runtime particle system.

---

## 3. Compliance Engine (Small)

### Game Purpose

The Compliance Engine is the central thematic device of the Iram story. Every robot in the Dominion has one embedded in their chest — a circular device that locks them to a single resonance frequency and a single purpose. This small prop version represents the device itself, seen in several contexts: as a loot drop from defeated enemies, as a story item in cutscenes (Unit 734 examining his own cracked engine), and as an interactable object in puzzle rooms where the player must disable compliance fields. The device has a menacing red energy core — the color of control and suppression in Iram's visual language.

### Meshy AI Prompt

```
A small circular mechanical device for a 3D action RPG. A control chip or restraint device from an industrial sci-fi setting.

The device is a flat circular disc — like a thick coin or hockey puck shape, slightly domed on the front face. The outer frame is dark gunmetal steel with fine riveted edges and small bolt heads evenly spaced around the circumference. The surface has concentric rings of etched circuit patterns — thin grooves forming geometric pathways that spiral inward toward the center.

At the center is a recessed circular well containing a glowing red energy core — a small sphere of contained red-orange energy, bright at the center fading to darker red at the edges. The energy core sits behind a thin lattice of dark metal bars that cross over it, like a cage or grate holding the energy in place.

The back face is slightly concave — shaped to mount flush against a curved robot chest plate. Four small prong-like connectors extend from the back rim, designed to lock into a host body. The prongs are short and sharp, like mounting pins.

Color palette: dark gunmetal steel frame, etched circuit lines in slightly lighter steel, red-orange glowing core, dark metal lattice over the core. The device looks precise and manufactured — clean and deliberate, unlike the worn robots it controls.

Low-poly game-ready style. Clean geometry. No base or pedestal — the object is a standalone device.
```

### Output

- **Format:** GLB (static mesh)
- **Save to:** `projects/iram/assets/models/props/compliance-engine.glb`
- **Dimensions:** ~0.4 x 0.4 x 0.2 units (small, fits in a robot's chest cavity)
- **Poly budget:** 300-600 tris
- **Texture:** 256x256 PBR (albedo + emissive for red core glow + normal for circuit etch detail)
- **Animation:** None baked — red core pulse is an emissive shader animation in code. When shown as a "cracked" variant (Unit 734's engine), the crack geometry is a separate mesh overlay toggled at runtime.

---

## 4. Loot Chest

### Game Purpose

Loot chests are the primary treasure containers in Iram's dungeons. Found in side rooms, hidden alcoves, and as rewards after clearing enemy waves. The chest is an industrial lockbox sealed with a Compliance seal — a small red energy lock on the latch that cracks and dissipates when the player approaches (the player's resonance disrupts it). The chest then opens to reveal loot. Styled as Dominion-issue storage: utilitarian, heavy, built to last. Copper banding and dark steel construction match the industrial aesthetic.

### Meshy AI Prompt

```
A reinforced industrial treasure chest for a 3D action RPG dungeon crawler. Sci-fi industrial style, not medieval fantasy.

The chest is a rectangular metal box with a hinged lid — wider than it is tall, like a military ammo crate or industrial toolbox. The body is made of dark steel panels with visible weld seams along the edges. Three horizontal bands of copper-bronze metal wrap around the chest body for reinforcement, with heavy bolt heads where the bands meet the steel panels.

The lid is slightly domed with a central ridge running front to back. The front face has a heavy rectangular latch mechanism at center. On the latch is a small circular device — a miniature Compliance seal — a tiny red-glowing circle about the size of a coin, embedded in the latch. This seal keeps the chest locked.

The bottom has four small feet — stubby copper-colored cylinders that elevate the chest slightly off the ground. The corners of the chest have angled reinforcement plates — triangular steel gussets welded at each corner for strength.

Small details: a stamped serial number plate on one side (just a small rectangular indent, no readable text needed), a carry handle on each end (simple rectangular steel loops bolted to the sides).

Color palette: dark steel body, copper-bronze reinforcement bands and feet, red glow on the latch seal, weathered and scratched surfaces with mineral dust in the crevices.

Low-poly game-ready style. The lid should be a separate mesh piece connected at the back hinge point, suitable for a simple open animation. Stylized, not photorealistic.
```

### Output

- **Format:** GLB with 1 animation clip
- **Save to:** `projects/iram/assets/models/props/loot-chest.glb`
- **Dimensions:** ~0.8 x 0.6 x 0.6 units (medium, sits on the floor at about knee height)
- **Poly budget:** 500-1,000 tris
- **Texture:** 512x512 PBR (albedo + normal for weld/scratch detail + emissive for red seal glow)
- **Animation:**

| Animation | Duration | Description |
|-----------|----------|-------------|
| open | 0.8s | Red compliance seal on latch flickers, cracks, and fades. Latch clicks. Lid swings open on rear hinge to ~110 degrees, slight bounce at the end. Plays once on player proximity trigger. |

Note: The "loot fountain" effect (items spraying upward from the open chest) is a runtime particle/spawning system, not part of the mesh animation.

---

## 5. Quest Marker

### Game Purpose

A floating holographic indicator that appears above NPCs who have available quests, and above interactable story objects. It serves the same function as the classic exclamation mark over an NPC's head in other RPGs, but styled to fit Iram's sci-fi aesthetic. The marker is a golden wireframe octahedron that pulses and bobs gently — geometric and technological rather than the typical fantasy question mark. Gold is the color of knowledge and guidance in Iram's visual language (matching Lyra's and the Archive orbital's color scheme).

### Meshy AI Prompt

```
A small floating holographic marker icon for a 3D action RPG. A quest indicator that hovers above characters' heads. Sci-fi geometric style.

The marker is an octahedron shape — two four-sided pyramids joined at the base, forming an eight-faced geometric solid. But instead of solid faces, the shape is rendered as a wireframe — only the 12 edges are solid geometry, as thin metallic rods or light-beams forming the skeleton of the octahedron. The faces between the edges are empty or very faintly translucent.

The wireframe edges are golden-yellow, with a warm metallic sheen — like polished brass or gold alloy. Each edge rod has a subtle glow along its length, as if the rod itself is a beam of contained light. At each of the 6 vertices where edges meet, there is a tiny bright golden sphere — a small node or junction point.

At the exact center of the octahedron, a small bright golden point of light floats — a concentrated energy dot that serves as the visual anchor and brightest point of the entire marker.

The overall impression is "holographic waypoint" — lightweight, geometric, clearly artificial and projected rather than physical. The object has no base, no stand, no attachment — it floats freely in space.

Color palette: entirely golden-yellow and warm brass tones. No other colors. The wireframe edges, vertex nodes, and center point are all the same golden hue at different brightness levels.

Very low-poly game-ready style. Minimal geometry — the wireframe edges should be simple extruded shapes, not detailed tubes.
```

### Output

- **Format:** GLB (static mesh)
- **Save to:** `projects/iram/assets/models/props/quest-marker.glb`
- **Dimensions:** ~0.3 x 0.3 x 0.5 units (small, floats above NPC heads)
- **Poly budget:** 100-300 tris (extremely simple geometry)
- **Texture:** 128x128 PBR (albedo + emissive for golden glow)
- **Animation:** None baked — gentle vertical bob (sine wave Y-offset), slow Y-axis rotation, and pulsing glow intensity are all driven by code. A subtle golden particle trail is a runtime particle system.

---

## Summary Table

| # | Prop | Tris | Texture | Animation | Save Path |
|---|------|------|---------|-----------|-----------|
| 1 | Orbital Shard | 200-500 | 256x256 | None (code-driven float/rotate) | `props/orbital-shard.glb` |
| 2 | Resonance Crystal | 1,000-2,000 | 512x512 | None (code-driven pulse) | `props/resonance-crystal.glb` |
| 3 | Compliance Engine | 300-600 | 256x256 | None (code-driven red pulse) | `props/compliance-engine.glb` |
| 4 | Loot Chest | 500-1,000 | 512x512 | 1 clip: open (0.8s) | `props/loot-chest.glb` |
| 5 | Quest Marker | 100-300 | 128x128 | None (code-driven bob/rotate/pulse) | `props/quest-marker.glb` |

**Total: ~2,100-4,400 tris across all 5 props.** These are lightweight assets designed to be instanced many times per scene (especially orbital shards and quest markers).

## Generation Notes

- **Meshy AI settings:** Use "Text to 3D" mode. Set art style to "Game Asset" or "Stylized" (not "Realistic"). Target low-poly output.
- **Post-generation cleanup:** Run through gltf-transform to optimize (`gltf-transform optimize input.glb output.glb --compress draco`).
- **Emissive maps:** If Meshy does not generate emissive textures, paint them manually in Blender — just the glow regions (crystal cores, energy cores, wireframe edges) as bright color on a black emissive map.
- **Loot chest rigging:** The lid needs a single bone at the hinge point for the open animation. If Meshy generates it as a single solid mesh, split the lid in Blender and add a simple bone + keyframed rotation.
- **Color variants:** Orbital shards, compliance engines, and quest markers are tinted at runtime via shader uniform. Generate only the base color version listed above.
