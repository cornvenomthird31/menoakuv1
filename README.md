# Kampung Ceria — Cozy Malaysian Village Game

A free, beginner-friendly browser game prototype built with plain HTML, CSS and JavaScript. No framework, game engine, paid assets or build tools are required.

## Play locally
1. Download or clone this folder.
2. Open `index.html` in a modern browser.
3. Move with **WASD** or the **arrow keys**. On mobile, use the on-screen direction pad.
4. Stand next to an object or weed and press **Space** / **Interact**.
5. Press **Sleep** to start a new day, restore energy and grow crops.

## Publish free with GitHub Pages
1. Create a free GitHub account at https://github.com/ if you do not have one.
2. Create a new public repository, for example `kampung-ceria`.
3. Upload `index.html`, `style.css`, `game.js` and this `README.md` to the repository root.
4. Open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch `main`, folder `/ (root)`, then Save.
7. Wait for GitHub Pages to publish. Your game URL will look like `https://YOUR-USERNAME.github.io/kampung-ceria/`.

## Files
- `index.html` — game page and user interface.
- `style.css` — layout, colours, responsive/mobile styling.
- `game.js` — canvas drawing, player movement, interactions, farming, fishing, restoration, energy, day cycle and local save system.

## Current prototype features
- Top-down pixel-style Malaysian village map drawn directly with Canvas.
- Player movement and interaction system.
- Energy/stamina and sleep/day cycle.
- Weed clearing, wood collection and village spirit points.
- Seed planting, watering, crop growth and harvesting.
- Fishing with random catch outcomes.
- Restore home, community hall, schoolhouse, bridge and carp pond.
- Inventory, task journal, map panel and automatic browser save.

## Important notes / next development steps
This is a playable first prototype, not yet a complete commercial-scale game. The current farm interaction uses a starter plot; a future version can add a full tile-based farming system, more crop types and seasonal rules, fishing minigame, bug-catching minigame, villagers and dialogue, shop/economy, quests, sound, richer pixel-art sprites, save slots and a larger explorable map. The Google Fonts import is optional; the game uses a system sans-serif fallback if offline.

## Reset your save
Open the browser developer console and run:
```js
localStorage.removeItem('kampungCeriaSave');
location.reload();
```
