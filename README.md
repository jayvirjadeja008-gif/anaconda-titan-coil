# ANACONDA: TITAN COIL
### *Eat the City. Coil the Sky.*

[![WebGL 3D](https://img.shields.io/badge/WebGL-Three.js_r128-00ffcc?style=for-the-badge&logo=three.js)](https://threejs.org/)
[![Web Audio API](https://img.shields.io/badge/Audio-Web_Audio_Synth-ff00aa?style=for-the-badge)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-v3.4-38bdf8?style=for-the-badge&logo=tailwindcss)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

An arcade-grade, full-screen **3D WebGL giant snake city destruction simulation game**. Control a massive, hyper-realistic green anaconda as it coils around skyscrapers, slithers across planetary highways, crushes enemy military defenses, and evolves into an apex cybernetic titan.

---

## 🎮 Play Live
- **GitHub Repository**: [https://github.com/jayvirjadeja008-gif/anaconda-titan-coil](https://github.com/jayvirjadeja008-gif/anaconda-titan-coil)
- **GitHub Pages**: Once enabled in repo Settings -> Pages -> Deploy from branch `main` (`/` root), the game is live at `https://jayvirjadeja008-gif.github.io/anaconda-titan-coil/`

---

## 🌟 Key Features

### 1. 🐍 Authentic Procedural Anaconda Anatomy & Physics
- **Realistic S-Wave Locomotion**: 40+ dynamic body segments undulating with propagating transverse sine waves and natural head leading orientation.
- **GLSL Keratin Scale Shader**: Procedural diamond-interlocking keratin scale shader with dark oval dorsal saddles, golden-ochre rings, cream belly scutes, and wet specular muscle shine.
- **4 Selectable Snake Morphs**:
  - 🐍 **Green Anaconda** (*Eunectes murinus*): Classic Amazonian camouflage with golden eye slits.
  - ⚡ **Cyber Neon**: Midnight carbon scales with pulsing electric cyan & hot-magenta hex veins.
  - 🌋 **Magma Drake**: Volcanic basalt scales with incandescent molten lava fissures.
  - 👑 **Solar Orochi**: Pearl-white scales with shimmering 24k gold diamond patterns and ruby eyes.

### 2. ☀️ Daylight Metropolis (Light Mode) & 🌙 Cyberpunk Night
- **Dynamic 3D Atmosphere Shift**: Seamlessly switch between bright, sunny high-noon daylight and neon-drenched cyberpunk night with **`L`** key or the UI toggle.
- **Sun & Moon Transitions**: The neon pink moon transforms into a radiant golden sun with an active solar corona ring.
- **Frosted Light HUD**: High-contrast, clean frosted ceramic UI skin with emerald telemetry indicators.

### 3. 🔊 Universal Audio & Procedural Synthesizer
- **Zero-Asset Web Audio API Engine**: Dynamic basslines, acid spit sweeps, crunch mastication, building rubble explosions, and alert arpeggios generated entirely in real time.
- **One-Click Sound Toggle**: Instant mute/unmute accessible on the Title Screen, in-game HUD, Pause menu, or via the **`M`** hotkey.
- **Master Gain Clamp**: Hardware-level instantaneous silence with `localStorage` memory.

### 4. 💥 Tactical Arcade Combat & Carnage Streaks
- **Constriction Crushing**: Wrap around skyscrapers and hold **`E`** to crush structures into tumbling concrete debris.
- **3D Floating Action Popups**: Real-time floating damage, points, and ability notifications (`+100 CHOMP!`, `💥 CRUSH! +800`, `⚡ TERMINATED!`).
- **Carnage Streak Multiplier**:
  - **3x**: `⚡ 3x HUNTER STREAK!`
  - **7x**: `🔥 7x APEX PREDATOR!`
  - **12x**: `👑 12x TITAN OMNIVORE!` (triggers Fire Rampage invincibility & camera shockwave).
- **Abilities**:
  - **Acid Venom Spit (`Q`)**: Long-range corrosive projectile that melts tanks and drone swarms.
  - **Tail Smash (`F`)**: Kinetic ground shockwave that shatters nearby ground units.
  - **Thermal Predator Vision (`R`)**: Heat-signature highlight with cinematic slow-motion tracking.
  - **Skin Shedding (`X`)**: Leaves behind a decoy husk while restoring full health.

---

## 🕹️ Controls Reference

| Action | Keyboard / Mouse | Touch / Mobile |
| :--- | :--- | :--- |
| **Steer Left / Right** | `A` / `D` or `Left` / `Right` Arrow (or Mouse Auto-steer) | Left Analog Joystick |
| **Sprint / Speed Boost** | Hold `Shift` | Hold `SPRINT` |
| **Jump / Aerial Leap** | `Spacebar` | Tap `JUMP` |
| **Wrap & Squeeze Structure** | Hold `E` near buildings | Hold `SQUEEZE` |
| **Acid Venom Spit** | `Q` | Tap `VENOM` |
| **Tail Smash / Shockwave** | `F` | Tap `SMASH` |
| **Thermal Heat Vision** | `R` (Slow-motion prey highlight) | Tap `HEAT` |
| **Shed Skin** | `X` (Full heal + decoy husk) | Ability Cluster |
| **Toggle Mute / Unmute** | **`M`** (or Click Mute Button) | Tap `[ 🔊 SOUND ]` |
| **Toggle Light / Night Mode** | **`L`** (or Click Theme Button) | Tap `[ ☀️ DAYLIGHT ]` |
| **Toggle Fullscreen** | Click `[ ⛶ FULLSCREEN ]` | Click `[ ⛶ FULLSCREEN ]` |
| **Pause Game** | `Escape` or `P` | Tap `[ ⏸ PAUSE ]` |

---

## 🛠️ Local Development & Quickstart

### Prerequisites
- Modern web browser (Chrome, Edge, Safari, Firefox) with WebGL and Web Audio API support.
- Node.js 18+ (optional, for development server).

### Running Locally (Zero Build Dependencies)
You can directly open `index.html` in any browser or serve it using Python:
```bash
python3 -m http.server 4173
# Open http://localhost:4173/
```

### Running with Vite
```bash
cd frontend
npm install
npm run dev      # Local dev server at http://localhost:5173/
npm run build    # Production build to dist/
npm run preview  # Preview production build at http://localhost:4173/
```

---

## 📐 Architecture & Technology Stack

```
+-------------------------------------------------------------+
|                     ANACONDA: TITAN COIL                    |
+-------------------------------------------------------------+
                               |
        +----------------------+----------------------+
        |                                             |
        v                                             v
[Three.js WebGL Engine]                     [Web Audio API Engine]
  - Procedural Spherical Planet               - Dynamic 8-step bassline
  - Custom GLSL Scale Shader                  - Procedural white noise burst
  - InstancedMesh 4-District City             - Frequency-ramping synth sweeps
  - Floating 3D -> 2D HUD Projection          - Master Gain Zero-Leak Mute
        |                                             |
        +----------------------+----------------------+
                               |
                               v
                  [Arcade State Machine]
                    - Fixed-dt Physics loop (60 FPS)
                    - District Progression & Boss Spawns
                    - Streak Multiplier & Mutation Upgrades
                    - localStorage High Scores & State
```

---

## 📜 License
Distributed under the **MIT License**. Free for commercial and non-commercial use.
