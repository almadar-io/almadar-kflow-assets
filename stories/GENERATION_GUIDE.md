# Knowledge Stories — Image Generation Guide

> ~120 images total: 11 covers + 55 scene illustrations + 10 game sprites + ~44 puzzle assets (headers, icons, backgrounds).
> Shared assets (terrain, effects, audio, world map) are already live on CDN — no generation needed.

---

## Visual Style — Illuminated Manuscript Futurism

All generated images MUST use the canonical **Illuminated Manuscript Futurism** style defined in `projects/iram/style.json`. This is the visual identity for all Almadar knowledge content.

### Master Style Prompt

Every image prompt is assembled as: `globalPrefix + domainPrefix + contentDescription + qualitySuffix`

**Global Prefix** (prepend to EVERY prompt):
> illuminated manuscript futurism, hand-painted vellum aesthetic, Celtic knotwork and Islamic geometric metalwork, warm amber and bone-ivory palette with teal accent, cinematic painterly composition, volumetric dust and warm mine-lamp glow, matte surfaces no chrome no plastic, no text no words no letters no numbers no writing no captions no labels no signatures

**Quality Suffix** (append to EVERY prompt):
> concept art, game concept art, painterly, intricate detail, ornate metalwork, vellum texture, aged parchment tones

**Negative Prompt** (use for EVERY generation):
> wrong colors, wrong body type, inconsistent design, different armor, text, words, letters, numbers, writing, captions, labels, signatures, typography, photorealistic, photograph, 3D render, CGI, anime, manga, cartoon, sketch, flat design, vector art, neon colors, blue tones, green vegetation, chrome metal, plastic surfaces, smooth untextured walls, modern technology, bright lighting, clean surfaces, extra limbs, extra fingers, fused fingers, malformed hands, missing limbs, asymmetric face, floating limbs, poorly drawn hands, anatomically incorrect, disfigured, blurry, low resolution, jpeg artifacts, noise, oversaturated, washed out, flat colors, muddy colors, pixelated, cropped head, out of frame, bad framing, overexposed, underexposed, flat lighting, speech bubble, text overlay, caption, subtitle, watermark, logo, HUD, UI element, studio white background

### Domain Prefixes

Each story domain adds a thematic layer on top of the global style:

| Domain | Prefix |
|--------|--------|
| **science** | scientific instruments visible, clean educational overlays, observatory/laboratory setting |
| **history** | ancient civilization setting, weathered stone and aged bronze, historical warfare/trade |
| **engineering** | mechanical blueprints visible, brass gears and structural diagrams, workshop/forge setting |
| **tech** | glowing circuits and data streams rendered as geometric knotwork, server/terminal setting |
| **math** | geometric patterns and mathematical curves rendered as illuminated marginalia |

### Example: Assembled Prompt

For "The Hot Gates" cover (history domain):

> illuminated manuscript futurism, hand-painted vellum aesthetic, Celtic knotwork and Islamic geometric metalwork, warm amber and bone-ivory palette with teal accent, cinematic painterly composition, volumetric dust and warm mine-lamp glow, matte surfaces no chrome no plastic, no text no words no letters no numbers no writing no captions no labels no signatures, ancient civilization setting, weathered stone and aged bronze, historical warfare/trade, an ancient Greek narrow mountain pass between sheer sea cliffs where a small band of bronze-armored Spartan warriors stands in phalanx formation against an endless tide of Persian soldiers stretching to the horizon dramatic painterly warm sunset lighting, concept art, game concept art, painterly, intricate detail, ornate metalwork, vellum texture, aged parchment tones

**Negative prompt**: (use the full negative prompt above)

### Cinematography Defaults

- **Lens**: 35mm wide angle
- **Depth of field**: deep focus
- **Lighting**: practical orange lamp light, volumetric light rays, rim lighting
- **Grain**: fine film grain

---

## What's Already Done (Shared Assets — DO NOT regenerate)

| Category | Count | Location | Used By |
|----------|-------|----------|---------|
| Isometric terrain tiles | 250+ | `shared/terrain/Isometric/` | Silk Road adventure, Hot Gates battle |
| Hex terrain tiles | 95 | `shared/hex-tiles/` | Future hex-based games |
| Particle effects | ~80 | `shared/effects/particles/` | Battle (Hot Gates), Physics Lab |
| Explosion animations | ~20 | `shared/effects/explosions/` | Battle games |
| Audio SFX | 26 | `shared/audio/sfx/` | All stories (step, answer, complete) |
| Background music | 6 | `shared/audio/music/` | All stories (by domain) |
| World map features | 12 | `shared/world-map/` | Silk Road adventure |
| 3D character models | 11 | `shared/models/characters/` | Trait Wars (not used by knowledge stories) |

## Style Guidelines

### Cover Images (1280x720, 16:9)
- Cinematic, evocative, painterly
- Domain-appropriate palette (warm for history, cool for tech, clean for science/math)
- Title-safe zone: keep top 20% and bottom 20% uncluttered for text overlay

### Scene Illustrations (1024x768, 4:3)
- Consistent style within a story (all 5 scenes should feel cohesive)
- Educational clarity over artistic complexity
- Diagrams/infographics welcome for STEM stories

### Game Sprites (256x256, transparent PNG)
- Flat or isometric style matching the game board
- Clear silhouette at small sizes (64px)
- Transparent background

---

## Story 1: The Hot Gates (`the-hot-gates`)
**Domain**: history | **Game**: battle | **Palette**: warm bronze/gold, deep red, Mediterranean blue

### Cover
> An ancient Greek narrow mountain pass between sheer sea cliffs, where a small band of bronze-armored Spartan warriors stands in phalanx formation against an endless tide of Persian soldiers stretching to the horizon. Dramatic, painterly, warm sunset lighting.

### Scene 1: The Persian Advance
> A vast Persian army stretching to the horizon across arid terrain, with columns of soldiers, cavalry, and war chariots approaching a narrow coastal mountain pass. Epic scale, viewed from above.

### Scene 2: The Narrow Pass
> A narrow coastal passage barely 12 meters wide squeezed between sheer rocky cliffs on one side and the Aegean sea on the other, bathed in golden light. A handful of armored warriors block the only way through.

### Scene 3: The Phalanx
> Greek hoplites in tight phalanx formation, interlocking bronze shields forming an impenetrable wall with spears protruding forward, filling the width of a narrow rocky pass. Close-up, dramatic angle.

### Scene 4: Three Days of Battle
> Exhausted Persian warriors in light armor falling before a disciplined wall of Spartan shields and spears in a narrow rocky pass, bodies and broken weapons scattered on the ground. Gritty and intense.

### Scene 5: The Lesson of Terrain
> A stylized tactical diagram showing a narrow bottleneck where only a few attackers can engage at once, with arrows illustrating how superior numbers are funneled and neutralized. Educational, clean design overlaid on a mountain pass landscape.

### Game Sprites (4)
| File | Description |
|------|-------------|
| `game/leonidas.png` | Spartan king — bronze Corinthian helmet with transverse crest, red cape, round aspis shield |
| `game/hoplite.png` | Greek hoplite soldier — bronze armor, round shield, long spear |
| `game/immortal.png` | Persian Immortal elite warrior — ornate light armor, spear, wicker shield |
| `game/archer.png` | Persian archer — light robes, composite bow, quiver |

---

## Story 2: The Silk Road (`the-silk-road`)
**Domain**: history | **Game**: adventure | **Palette**: warm amber/gold, desert ochre, oasis green

### Cover
> A merchant's camel caravan traversing a vast desert landscape at sunset, with distant oases and snow-capped mountain passes visible on the horizon. Silk bales and spices loaded on camels, starlit sky emerging. Rich, warm palette evoking ancient Central Asian trade routes.

### Scene 1: The Merchant's Departure
> A merchant loading camels with silk bales, porcelain, and tea at the grand gates of ancient Chang'an (Xi'an), with traditional Chinese architecture, bustling market activity, and a long road stretching into the distance.

### Scene 2: Oasis Navigation
> A small caravan of camels navigating between green palm-lined oases at the edge of the vast Taklamakan Desert, the contrast between deadly dunes and life-giving water vivid and stark.

### Scene 3: The Network Effect
> A stylized bird's-eye map showing multiple interconnected trade routes across Central Asia, with cities as glowing nodes and routes as connecting edges, mountains and deserts forming natural barriers between paths.

### Scene 4: Knowledge Transfer
> Merchants of diverse origins exchanging scrolls, astronomical instruments, spices, and glassware inside a bustling Silk Road caravansary, with arched stone architecture and warm lamplight.

### Scene 5: The Graph Lesson
> An abstract graph theory visualization overlaid on a Silk Road map, with city nodes connected by weighted edges showing distance, danger ratings, and cost. Clean educational style.

### Game Sprites (1)
| File | Description |
|------|-------------|
| `game/marco.png` | Merchant traveler — robes, turban, travel pack, for hex adventure map. Top-down or isometric. |

**Shared asset reuse**: Terrain tiles (desert, plains, oasis, mountains, city) + world map features (oasis, city, banditCamp, treasure, start, goal) are all already in `shared/`.

---

## Story 3: The Smart Thermostat (`the-smart-thermostat`)
**Domain**: engineering | **Game**: event-handler | **Palette**: clean blue/white, warm orange accents

### Cover
> A modern smart thermostat on a living room wall displaying 21°C, with abstract flowing arrows showing the feedback loop between temperature sensor, heater, and fan. Clean, technical illustration style with warm domestic lighting.

### Scene 1: The Feedback Loop
> A detailed illustration of James Watt's centrifugal governor on a brass steam engine, with spinning metal balls connected to a valve mechanism, steam rising. Historical-technical crossover style.

### Scene 2: Events and Handlers
> A clean diagram showing temperature events (thermometer icons rising and falling) connected by directional arrows to heater and fan action icons, with event labels. Technical blueprint aesthetic.

### Scene 3: The Hysteresis Band
> A temperature-over-time graph showing wild oscillation without hysteresis (left) contrasted with smooth, stable control within a 19-23°C dead band (right). Clean data visualization style.

### Scene 4: Composition of Rules
> Multiple event-handler rule cards combining like puzzle pieces into a complex smart home control panel, showing if-then logic chains connecting sensors to actuators. Infographic style.

### Scene 5: From Thermostats to Software
> A split-view illustration with a physical thermostat and heating system on the left, and a modern event-driven software architecture diagram (event bus, handlers, state) on the right, connected by visual parallels.

### Game Sprites (3)
| File | Description |
|------|-------------|
| `game/thermometer.png` | Digital thermometer sensor — clean icon style, shows temperature reading |
| `game/heater.png` | Heating unit/radiator — warm orange glow, mechanical feel |
| `game/fan.png` | Cooling fan/AC unit — blue-tinted, spinning blade iconography |

---

## Story 4: The Traffic Light (`the-traffic-light`)
**Domain**: engineering | **Game**: state-architect | **Palette**: traffic green/yellow/red, dark urban backdrop

### Cover
> A traffic light at a busy intersection cycling through green, yellow, and red, with an abstract state machine diagram (three connected circles with arrows) superimposed over the scene. Urban night setting with car headlights streaking by.

### Scene 1: Before Traffic Lights
> A Victorian-era gas-lit traffic semaphore with a uniformed police officer operating it, next to a modern three-color traffic light for comparison. London street scene, 1868 atmosphere.

### Scene 2: Why Two States Fail
> A dramatic split illustration showing a two-state traffic light causing a car collision on the left, versus a three-state light with smooth safe transitions on the right. Clear cause-and-effect visual.

### Scene 3: The State Machine
> A clean state diagram with three colored circles (GREEN, YELLOW, RED) connected by arrows labeled "TIMER", forming a cycle. Crisp, educational diagram on a dark background.

### Scene 4: Adding Emergency
> A state machine diagram where a red "EMERGENCY" arrow points from every state (GREEN, YELLOW) directly to RED, with an ambulance icon as the trigger. Clear, technical illustration.

### Scene 5: State Machines Everywhere
> A collage showing four mini state machine diagrams: a vending machine, an elevator, a TCP handshake, and a game character's states (IDLE, WALKING, ATTACKING, DEAD). Clean, consistent diagram style.

### Game Sprites: None needed (pure diagram interaction)

---

## Story 5: The Perfect Throw (`the-perfect-throw`)
**Domain**: science | **Game**: physics-lab | **Palette**: sky blue/sunset gradient, clean white annotations

### Cover
> A ball in mid-flight tracing a perfect parabolic arc against a twilight sky, with faint angle markings showing 45 degrees from the launch point. Galileo's silhouette visible in the background with an inclined plane. Scientific and elegant.

### Scene 1: Galileo's Ramps
> Galileo in a Renaissance workshop rolling bronze balls down inclined wooden planes, with a water clock dripping in the foreground and scattered notes with mathematical sketches. Warm candlelit atmosphere.

### Scene 2: Two Motions, One Trajectory
> A parabolic trajectory of a ball decomposed into a constant horizontal arrow and an accelerating vertical arrow, with dotted lines showing the independent components combining into the curve. Physics textbook illustration style.

### Scene 3: The Angle Trade-off
> Three trajectories from the same launch point: a low flat arc at 15° (short), a perfect parabola at 45° (farthest), and a steep high arc at 75° (tall but short range). Clean vector style with angle labels.

### Scene 4: The Range Equation
> The range equation R = v²sin(2θ)/g written on a chalkboard, with side-by-side trajectory comparisons on Earth (short) and the Moon (very long) for the same throw. Educational, physics classroom feel.

### Scene 5: Real-World Complications
> Different projectiles shown at their real-world optimal angles: a baseball at 35°, a golf ball at 12° with backspin lines, and a javelin at 30°, each with air resistance streamlines. Sport-science infographic style.

### Game Sprites (2)
| File | Description |
|------|-------------|
| `game/ball.png` | Projectile ball — clean, round, slight motion blur trail |
| `game/target.png` | Landing target/platform — bullseye or landing zone marker |

---

## Story 6: The $125 Million Bug (`the-125-million-bug`)
**Domain**: science | **Game**: sequencer | **Palette**: deep space black, Mars rust-red, warning amber

### Cover
> The Mars Climate Orbiter spacecraft glowing with atmospheric friction as it descends too close to Mars, with a faint overlay of the equation "1 lbf·s = 4.448 N·s" and warning indicators. Dramatic space scene with Mars looming large and red.

### Scene 1: Two Teams, One Mission
> Two teams of engineers working in separate offices — one with imperial measurement charts on the wall (Denver), the other with metric/SI charts (Pasadena). Split-screen composition showing the disconnect.

### Scene 2: Launch and the Long Journey
> A spacecraft cruising through deep space with small thruster firings shown as tiny bursts, with faint trajectory lines subtly diverging from the planned path. Dark, vast space backdrop.

### Scene 3: The Deviations Grow
> A graph showing predicted trajectory (solid line) versus actual trajectory (dashed line) slowly diverging over 9 months, with small correction arrows that compound the error. Data visualization style.

### Scene 4: 57 Kilometers Too Close
> A spacecraft glowing red-hot from atmospheric friction as it plunges into the thin Martian atmosphere far too close to the rust-colored surface, breaking apart. Dramatic, cinematic space disaster scene.

### Scene 5: The Post-Mortem
> Engineers gathered around a whiteboard showing the equation 1 lbf·s = 4.448 N·s circled in red marker, with somber expressions. The failed mission timeline visible on a screen behind them.

### Game Sprites: None needed (card ordering interaction)

---

## Story 7: The Bridge That Swayed (`the-bridge-that-swayed`)
**Domain**: engineering | **Game**: builder | **Palette**: steel grey/blue, Thames slate, modern London

### Cover
> London's Millennium Bridge packed with pedestrians visibly swaying side to side, with St Paul's Cathedral in the background and the Thames below. Abstract resonance wave patterns overlaid on the bridge deck. Dramatic, slightly unsettling atmosphere.

### Scene 1: Grand Opening
> A sleek, modern pedestrian suspension bridge over the Thames on a bright sunny day, packed with thousands of excited people crossing. St Paul's Cathedral on one side, Tate Modern on the other.

### Scene 2: The First Wobble
> Pedestrians on a bridge visibly lurching and grabbing handrails with alarmed expressions, the bridge deck tilting slightly to one side. Motion blur suggesting lateral sway.

### Scene 3: Synchronized Walking
> An overhead bird's-eye view of a crowd on a bridge, their feet all stepping in the same direction simultaneously. Motion arrows showing the positive feedback loop: bridge sways → people sync → sway increases.

### Scene 4: Engineers Investigate Resonance
> Engineers with measurement equipment and accelerometers on an empty bridge, laptop screens showing frequency analysis graphs with a peak at 1 Hz. Technical investigation scene.

### Scene 5: The Damper Solution
> Engineers installing large mechanical tuned mass damper devices and viscous dampers underneath a bridge deck, with technical cross-section diagrams showing the counter-oscillation mechanism.

### Game Sprites: None needed (component placement on blueprint)

---

## Story 8: The Invisible Hand (`the-invisible-hand`)
**Domain**: science | **Game**: simulator | **Palette**: warm market colors, storybook warmth, parchment tones

### Cover
> A bustling village marketplace with two bakeries facing each other across a narrow cobblestone street, price signs being updated, and villagers choosing between them. Warm, storybook illustration style with supply-and-demand curves subtly drawn in the sky.

### Scene 1: The Village Baker
> A single bakery on a quiet village street with a long queue of villagers waiting outside. The baker inside looks content and prosperous. A price sign reads "4 coins." Medieval/fairytale village atmosphere.

### Scene 2: A Competitor Arrives
> Two bakeries facing each other across a cobblestone street, both with price signs being hastily updated — one crossing out "4.0" and writing "3.5", the other showing "3.0". Competitive energy.

### Scene 3: Price War
> An animated supply and demand graph with two curves dynamically shifting, arrows converging on an intersection point. Village marketplace in the background as prices drop.

### Scene 4: Finding Equilibrium
> A balanced scale with "Supply" on one side and "Demand" on the other, perfectly balanced at 2.50 coins. The village thrives in the background with both bakeries busy and happy customers.

### Scene 5: The Invisible Hand
> A bustling village market with multiple vendors, happy customers, and invisible flowing golden lines connecting supply and demand. A ghostly hand shape formed by the market flows.

### Game Sprites: None needed (slider/parameter interaction)

---

## Story 9: The Merchant's Scale (`the-merchants-scale`)
**Domain**: history | **Game**: classifier | **Palette**: warm gold, aged wood, lamplight amber

### Cover
> A medieval merchant in an ancient workshop carefully lowering a gold coin into a graduated glass vessel of water, with a balance scale and scattered coins on a wooden counter. Warm lamplight, Archimedes-era atmosphere.

### Scene 1: The Merchant's Dilemma
> A medieval merchant at a worn wooden counter with a brass balance scale, examining a gold coin suspiciously under lamplight. Stacks of coins and olive oil amphorae in the background.

### Scene 2: Archimedes and the King's Crown
> An ancient Greek mathematician in a toga deep in thought staring at an ornate golden crown on a marble table, scrolls and geometric instruments scattered around.

### Scene 3: The Eureka Moment
> A man in an ancient bath, water overflowing the edges as he lowers himself in, having a sudden moment of realization. Water splashing onto a tiled floor.

### Scene 4: Water Displacement
> Two identical water vessels side by side — one containing a crown, the other a gold bar of equal weight — showing clearly different water levels. Clean, educational comparison.

### Scene 5: Testing the Coins
> A merchant carefully lowering a gold coin into a graduated glass vessel filled with water, measuring the displacement with precise markings. Close-up, warm workshop lighting.

### Game Sprites: None needed (card sorting interaction)

---

## Story 10: The Password That Wasn't (`the-password-that-wasnt`)
**Domain**: tech | **Game**: debugger | **Palette**: dark blue/black, neon green terminal, red warning accents

### Cover
> A security auditor at a laptop in a dimly lit server room, database records with hash values visible on the screen, a cracked padlock icon glowing red. Cybersecurity aesthetic with dark blues and neon highlights.

### Scene 1: The Breach
> A security auditor at a laptop in a dark office, database records scrolling on screen showing hash values like "5f4dcc3b5aa765d61d8327deb882cf99". Green terminal text reflected in glasses.

### Scene 2: Rainbow Tables
> A massive table visualization showing common passwords on the left and their MD5 hash values on the right, with one row highlighted and matched. Dark, data-dense aesthetic.

### Scene 3: Hash Functions Explained
> A diagram showing passwords entering a funnel labeled "HASH FUNCTION" and coming out as fixed-length hex strings. One-way arrows, no reverse path. Clean cryptography infographic.

### Scene 4: Why MD5 Fails
> A speedometer showing "10 BILLION hashes/sec" next to the MD5 logo, with a red warning triangle. GPU cards stacked behind. Alarming technical infographic.

### Scene 5: The Salt Solution
> A diagram showing a password combined with a random salt before being fed into bcrypt, with a clock showing "100ms per hash" versus MD5's "1 nanosecond." Secure vs insecure comparison.

### Game Sprites: None needed (code line inspection)

---

## Story 11: The Prisoner's Choice (`the-prisoners-choice`)
**Domain**: math | **Game**: negotiator | **Palette**: noir grey, cold blue, interrogation white

### Cover
> Two people in separate stark interrogation rooms divided by a wall, each facing a choice between two doors labeled "Cooperate" and "Defect." A 2x2 payoff matrix floats between them. Tense, dramatic noir lighting.

### Scene 1: The Arrest
> Two people being led into separate interrogation rooms by detectives, a concrete wall dividing them. Documents with "THE DEAL" on each table. Noir crime drama atmosphere.

### Scene 2: The Interrogation Room
> A person sitting alone in a cold interrogation room, agonizing over a decision. Two thought bubbles show outcomes: freedom (betrayal) versus 1 year (silence). Stark overhead lighting.

### Scene 3: Nash's Insight
> A 2x2 payoff matrix on a blackboard with four outcomes filled in, a mathematician's hand pointing to the Nash equilibrium cell (Defect/Defect). The (Cooperate/Cooperate) cell highlighted as better but unstable.

### Scene 4: The Iterated Game
> A timeline showing 10 rounds of a repeated game, with green (cooperate) and red (defect) circles forming patterns. Cooperation streaks and retaliation sequences visible.

### Scene 5: Axelrod's Tournament
> A tournament bracket showing strategy names (Tit-for-Tat, Always Defect, Random, Grudger, Pavlov) with Tit-for-Tat rising to the top as champion. Clean, celebratory infographic.

### Game Sprites: None needed (button choice interaction)

---

## Generation Checklist

For each story, drop files into `projects/kflow-assets/stories/{slug}/`:

```
stories/{slug}/
  cover.png          # 1280x720
  scenes/
    scene-1.png      # 1024x768
    scene-2.png
    scene-3.png
    scene-4.png
    scene-5.png
  game/              # only if sprites listed above
    {sprite}.png     # 256x256, transparent
```

After adding files:
1. `cd projects/kflow-assets`
2. `git add stories/{slug}/`
3. `git commit -m "assets: {slug} cover + scenes"`
4. `git push` → Firebase auto-deploys to CDN
5. Verify in Storybook — images appear immediately (code wiring is done)

## Priority Order (suggested)

1. **the-125-million-bug** — already wired in Storybook with `storySlug`, easiest to verify
2. **the-hot-gates** — battle game, most visually rich, also has Storybook variant
3. **the-silk-road** — adventure game, tests shared terrain/world-map reuse
4. Remaining 8 stories in any order
