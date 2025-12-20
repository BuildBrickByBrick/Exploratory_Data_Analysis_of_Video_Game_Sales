
<img width="1173" height="678" alt="image" src="https://github.com/user-attachments/assets/213ad1ad-5363-4d6c-88b0-bda33f202783" />
<img width="1184" height="673" alt="image" src="https://github.com/user-attachments/assets/698f38a2-7db0-41b3-8ad9-272614de57a6" />
<img width="1222" height="760" alt="image" src="https://github.com/user-attachments/assets/73df1ac1-e916-42bc-baef-088d585b0519" />
# INNER HELL: Psychological Survival Architect

**INNER HELL** is a high-performance, browser-based 2.5D retro-FPS engineered with a custom raycasting engine and powered by the **Google Gemini API**. It explores the intersection of psychological archetypes and procedural gameplay, manifesting user-defined fears into complex AI agents with unique behavioral traits.

## 🕹️ Technical Overview

The application is built on a high-speed TypeScript engine, prioritizing low-level graphical control and deep AI simulation without the overhead of modern 3D frameworks.

### 🏗️ Custom Raycasting Engine
- **District-Based Procedural Generation**: The engine generates a multi-district map of a ruined NYC (Financial District, Hotel Strip, Harlem-style Residential, Shopfronts, and Subways).
- **Z-Buffer Management**: Full Z-Buffer implementation for correct sprite-to-wall depth sorting and fog calculation.
- **Advanced Texture Mapping**: Uses exact "Wall-X" mapping to place procedural neons, windows, and urban grime.
- **Atmospheric Rendering**: Real-time fog, screen-shake (trauma), and palette-accurate lighting.

### 🧠 Personality-Driven AI System
Every enemy in *INNER HELL* is more than just a target. Using the **Gemini 2.5 Pro/Flash** models, the game generates a `Fear Profile` comprising 9 distinct personality traits:
- **Aggression / Impulsiveness**: Dictates state transitions to `CHARGING`.
- **Cowardice / PanicResponse**: Triggers `RETREATING` or `PANICKING` states based on player proximity.
- **Persistence / Awareness**: Influences `STALKING` and `FLANKING` behaviors.
- **DrainIntensity**: Determines the rate of willpower/health depletion during proximity.

### ⚡ Interactive Environmental Physics
The urban landscape is reactive to player input:
- **Dynamic Props**: Hitting a `brokenMonitor` triggers electric spark particles.
- **Kinematic Wires**: Shooting `hangingWire` props triggers a decaying phase-based swinging animation.
- **Hazard Interactivity**: `ExplosiveBarrels` feature a fused countdown and chain-reaction capabilities.

## 🛠️ Features

- **Generative Manifestation**: Enter any fear (e.g., "Student Loans", "The Deep Ocean", "Obsolescence") to generate a unique enemy type via Gemini API.
- **Diagnostic Scanner**: Real-time AI trait inspection (Hold `T`) to view the psychological stats of the entity currently targeted.
- **Arsenal Progression**: A 5-tier weapon system ranging from the *STREET-SAW* to the *CITY-CRUSHER* tank cannon.
- **Cyberpunk HUD**: Integrated real-time Minimap, health vitals, and willpower (score) tracking.

## ⌨️ Controls

| Key | Action |
| --- | --- |
| **W/A/S/D** | Locomotion (Move & Strafe) |
| **Mouse** | Look (Rotation) |
| **Mouse Left** | Discharge Weapon |
| **1 - 5** | Select Unlocked Arsenal Tier |
| **T (Hold)** | Activate Diagnostic Trait Scanner |
| **Click Canvas** | Lock Pointer & Resume Audio |

## 🚀 Installation & Setup

1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/inner-hell.git
    ```
2.  **Environment Variables**:
    The application requires an `API_KEY` for the Google Gemini SDK. Ensure your execution environment has `process.env.API_KEY` configured.
3.  **Local Execution**:
    The project uses ES6 modules. Serve the root directory via any local static server (e.g., `npx serve .`).

## 🧱 Project Structure

- `index.tsx`: Main React entry point and Gemini integration logic.
- `game/engine.ts`: Core 2.5D renderer, physics, and entity management.
- `game/audio.ts`: Procedural WebAudio synthesis for weapons, explosions, and UI.
- `game/types.ts`: Engine-wide interfaces and psychological trait definitions.

---
*Built for the edge of browser performance and the depths of human fear.*
