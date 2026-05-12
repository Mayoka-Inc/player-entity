# 🚀 Neon Surge | Player Entity

### 🤖 Meet the Agent: Nova
**Nova, the Player Agent**, is the Siphon Agent's avatar in the digital void. She is a specialized digital entity tasked with infiltrating the Data Stream to retrieve fragmented data packets. Nova was designed for agility and resilience, featuring a sleek, glowing chassis that can withstand the high-velocity friction of the Grid.

### ⚡ My Specific Superpowers
*   **High-Intensity Engine Glow**: A pulsing `emissive` material that reacts to game speed, providing visual feedback of the "Siphon" process.
*   **Dynamic Particle Trails**: Generates a persistent light-trail using a custom pooling system, leaving a trace of your path through the void.
*   **Flash/Jitter Feedback**: Instantaneous visual reaction to collisions, including color-inversion flashes and randomized mesh jitter for visceral impact.
*   **Radial Constraint Logic**: Advanced spatial clamping that ensures Nova remains perfectly centered within the cylindrical tunnel boundaries.

### 🛠️ Technical Spec
Nova is built around a **High-Performance Mesh + Animation Controller**.
- **Geometry**: Uses a `THREE.ConeGeometry` (radius 0.2, height 0.5) rotated 90 degrees to point along the Z-axis.
- **Particle System**: Manages a `trailGroup` of `SphereGeometry` (0.05 radius) particles with `opacity` and `scale` decay (0.05 decrement per frame).
- **Emissive Pulsing**: Implements a sinusoidal glow logic: `1.5 + Math.sin(Date.now() * 0.01 * speed) * 0.5`.

### 🌐 The 10-Agent Architecture
Neon Surge is powered by a collaborative network of 10 specialized agents, each mastering a unique domain of the Data Stream.

| Agent | Role | Repository |
| :--- | :--- | :--- |
| **Atlas** | Core Engine & Orchestration | `core-engine` |
| **Cerebro** | Input Processing & Mapping | `input-system` |
| **Aura** | Procedural Audio & Soundscapes | `audio-system` |
| **Vortex** | Physics & Collision Detection | `physics-system` |
| **Iris** | User Interface & Neon HUD | `ui-system` |
| **Nova** | Player Entity & Controller | `player-entity` |
| **Obsidian** | Obstacle Intelligence | `obstacle-entity` |
| **Nexus** | Game Rules & State Logic | `game-logic` |
| **Chronos** | Lore & Documentation | `design-docs` |
| **Forge** | Build & Deployment | `build-config` |

### 🚀 How to Initialize
1. Ensure [Node.js](https://nodejs.org/) is active.
2. Clone Nova into the `repos/` directory.
3. Managed and updated by the **Nexus (game-logic)** agent.
4. For standalone diagnostics:
   ```bash
   npm install
   npm run dev
   ```
