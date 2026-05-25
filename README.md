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

If you already have this folder locally, just open it in PowerShell:

```powershell
cd "D:\Muzammil\Misc\Projects & Dev\Neural Dungeon"
```

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

## Screenshots

Add screenshots to a `screenshots/` folder and link them here.

```text
screenshots/
+-- gameplay.png
+-- game-over.png
```

Example Markdown:

```markdown
![Gameplay](screenshots/gameplay.png)
![Game Over](screenshots/game-over.png)
```

## GitHub Publishing From PowerShell

Run these commands from PowerShell after you have reviewed the files:

```powershell
cd "D:\Muzammil\Misc\Projects & Dev\Neural Dungeon"

git init
git branch -M main
git status

git add README.md .gitignore neural-dungeon.html
git commit -m "Initial commit"

gh repo create neural-dungeon --public --source . --remote origin --push
```

Use `--private` instead of `--public` if you want the repository to be private:

```powershell
gh repo create neural-dungeon --private --source . --remote origin --push
```

## Files That Should Not Be Pushed

This project currently has no `.env` file, API key file, database file, dependency folder, or build output folder.

Do not push these if you add them later:

- `.env` or `.env.*`
- API keys, tokens, credentials, or private config files
- Local database files such as `.db`, `.sqlite`, or `.sqlite3`
- Dependency folders such as `node_modules/` or `vendor/`
- Build output folders such as `dist/`, `build/`, or `out/`
- Local editor folders such as `.vscode/` or `.idea/`
- Logs, archives, backups, and temporary files

## Author

Muzammil
