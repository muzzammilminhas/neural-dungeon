# Neural Dungeon

Neural Dungeon is a single-file HTML5 Canvas dungeon crawler game. It runs directly in a modern browser with no framework, build step, package manager, CDN, or external asset dependency.

## Features

- Fullscreen real-time dungeon crawler rendered with the Canvas 2D API
- Procedural dungeon generation using BSP-style room splitting and carved corridors
- Randomized runs seeded from browser randomness
- Player movement with `WASD` or arrow keys
- Mouse-based melee attacks and `Space` dodge movement
- Enemy types with different behavior:
  - Grunts chase and attack in melee range
  - Archers keep distance and fire projectiles
  - Sentinels patrol rooms with vision cones
- A* pathfinding for enemy navigation
- Health, score, kills, room multiplier, and active boost HUD
- Pickup items for health, speed, and damage boosts
- Fog-of-war minimap with explored rooms, enemies, player position, and exit marker
- Win and death overlay with dungeon regeneration
- Particle effects, screen shake, attack arcs, projectiles, and FPS meter
- Responsive layout for desktop and smaller screens

## Tech Stack

- HTML5
- CSS3
- JavaScript
- Canvas 2D API
- Web Crypto API for run seed entropy
- Browser DOM events for keyboard, mouse, resize, and UI interaction

## Folder Structure

```text
Neural Dungeon/
+-- neural-dungeon.html   # Complete game: HTML, CSS, and JavaScript
+-- README.md             # Project documentation
+-- .gitignore            # Files Git should ignore
```

## Installation

No dependency installation is required.

To get the project locally from GitHub later:

```powershell
git clone https://github.com/YOUR-USERNAME/neural-dungeon.git
cd neural-dungeon
```

If you already have this folder locally, just open it in by double-click:

## Run Commands

Run directly in your default browser:

```powershell
Start-Process ".\neural-dungeon.html"
```

Optional local server run, useful if you later add separate assets:

```powershell
python -m http.server 5500
```

Then open:

```powershell
Start-Process "http://localhost:5500/neural-dungeon.html"
```

## Controls

| Action | Control |
| --- | --- |
| Move | `WASD` or arrow keys |
| Attack | Left mouse click |
| Dodge | `Space` |
| Restart after win/death | `Regenerate Dungeon` button |

## Author

Muzammil
