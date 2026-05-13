<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=24&pause=1000&color=7aa2f7&center=true&vCenter=true&width=600&lines=Nova:+Running+Propulsion+Diagnostics...;Calibrating+Neural+Interface...;Nova+Pulse+Active." alt="Typing SVG" />
</div>

# 🚀 Neon Surge | Player Entity

### 📊 Agent Telemetry
<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=mayoka0&theme=tokyo-night&hide_border=true&area=true" width="100%" alt="Activity Graph" />
</div>

### 🤖 Meet the Agent: Nova
**Nova, the Player Agent**, is the Siphon Agent's avatar in the digital void. She is a specialized digital entity tasked with infiltrating the Data Stream to retrieve fragmented data packets. Nova was designed for agility and resilience, featuring a sleek, glowing chassis that can withstand the high-velocity friction of the Grid.

### ⚡ My Specific Superpowers
*   **High-Intensity Engine Glow**: A pulsing `emissive` material that reacts to game speed, providing visual feedback of the "Siphon" process.
*   **Dynamic Particle Trails**: Generates a persistent light-trail using a custom pooling system, leaving a trace of your path through the void.
*   **Flash/Jitter Feedback**: Instantaneous visual reaction to collisions, including color-inversion flashes and randomized mesh jitter for visceral impact.
*   **Radial Constraint Logic**: Advanced spatial clamping that ensures Nova remains perfectly centered within the cylindrical tunnel boundaries.

### 🛠️ Technical Spec
Nova is built around a **High-Performance Mesh + Animation Controller** optimized for high-speed traversal of the Data Stream. The entity's visual presence is defined by a `THREE.ConeGeometry` (radius 0.2, height 0.5) that points along the Z-axis, creating an aggressive, aerodynamic profile. This geometry is paired with a custom emissive material that pulses in response to the game's current speed. The pulsing logic follows a sinusoidal curve: `1.5 + Math.sin(Date.now() * 0.01 * speed) * 0.5`, providing a rhythmic visual cue of the agent's velocity.

A core technical challenge solved by Nova is the implementation of a **Custom Particle Pooling System** for its light trails. To avoid the overhead of frequent garbage collection, Nova pre-allocates a `trailGroup` of `SphereGeometry` particles. As the agent moves, these particles are recycled, with their `opacity` and `scale` values decaying by 0.05 every frame. Furthermore, Nova includes a robust **Radial Constraint Logic** layer. This mathematical clamp ensures that the player entity remains perfectly centered within the cylindrical tunnel's boundaries, regardless of extreme input maneuvers or physical impacts.

🔗 **Part of the [Neon Surge Ecosystem](https://github.com/mayoka0/mayoka0#-neon-surge-architecture)**

### 🚀 How to Initialize
1. Ensure [Node.js](https://nodejs.org/) is active.
2. Clone Nova into the `repos/` directory.
3. Managed and updated by the **Nexus (game-logic)** agent.
4. For standalone diagnostics:
   ```bash
   npm install
   npm run dev
   ```
