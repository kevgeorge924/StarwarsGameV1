## X-Wing Death Star Run (Mini 3D Shooter)

A small learning project: a simple 3D space shooter where you fly an X-Wing along a trench toward the Death Star exhaust port. The focus is on keeping the scope tiny and building the game in clear phases.

---

## Requirements (MVP)

- **Platform**
  - Runs in a desktop web browser (no installs).
  - Keyboard controls only (no gamepad required).

- **Gameplay Scope**
  - Single-player, single short trench run.
  - Simple health system (player can be destroyed).
  - Basic shooting (forward lasers).
  - A clear lose condition (crash or get shot).
  - A clear win condition (reach the end and hit the target).

- **Non-Goals (for now)**
  - No multiplayer.
  - No advanced physics.
  - No save system or progression.
  - No complex menus or settings.

---

## Tech Stack

To keep things simple and easy to run:

- **Runtime**: Web browser (modern desktop Chrome/Firefox/Edge/Safari).
- **Language**: JavaScript (ES modules).
- **3D Engine**: `three.js` (loaded from a CDN, no build step at first).
- **Assets**:
  - Placeholder geometry (boxes, cylinders) for the X-Wing and environment to start.
  - Simple colors and basic lights (no complex materials initially).

This choice avoids engine installers and lets us focus on core 3D/game concepts.

---

## Roadmap & Phases

We will build the game in small, focused phases. Each phase should be playable or testable before moving on.

- **Phase 1 — Project Setup & Empty Space Scene**
  - Create basic project structure (`index.html`, `main.js`).
  - Load `three.js` from a CDN.
  - Create a scene with camera, renderer, and a render loop.
  - Add a simple placeholder X-Wing (e.g., a box) in empty space.
  - Verify that the scene renders and the ship is visible.

- **Phase 2 — Basic Ship Movement & Camera**
  - Add continuous forward movement for the X-Wing.
  - Implement keyboard input for roll and slight yaw/pitch.
  - Add a following third-person camera that tracks the ship.
  - Ensure movement feels smooth and responsive.

- **Phase 3 — Trench Environment Blockout**
  - Build a simple trench using basic geometry (floor, walls).
  - Add basic lighting and a starfield/space backdrop.
  - Position the trench so the ship flies through it.

- **Phase 4 — Shooting & Collisions**
  - Implement primary fire (laser bolts).
  - Detect hits on simple targets or walls.
  - Add basic collision detection for the ship vs. trench walls.
  - Add visual feedback for hits (e.g., color flash, small particle-like effect).

- **Phase 5 — Enemies & Hazards**
  - Place simple turret objects along the trench.
  - Turrets periodically fire at the player in a basic pattern.
  - Introduce a small variety of obstacles (pillars, beams).

- **Phase 6 — Health, UI & Game Loop**
  - Player health and destruction when health reaches zero.
  - Simple HUD: health and maybe distance to end.
  - Basic restart flow (reload level or reset state).

- **Phase 7 — Exhaust Port & Victory**
  - Add an exhaust-port target at the end of the trench.
  - Implement a way to destroy it (well-placed shot or trigger).
  - Show a simple victory screen and optional score (time/damage).

- **Phase 8 — Polish (Optional)**
  - Replace placeholders with nicer models (still simple).
  - Add sound effects and simple music.
  - Tune difficulty and pacing.

---

## Current Status

- **Chosen tech**: Browser-based JavaScript + `three.js` (CDN).
- **Next step (Phase 1)**: Set up the basic web project and render a simple 3D scene with a placeholder X-Wing visible.

