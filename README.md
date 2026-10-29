# Zone 9 Prototype — Lobby + Map Explorer

Standalone Zone 9 first-person prototype with a Standoff 2 Remastered-inspired lobby/mode selector. This is a separate project and does not modify `standoffX/StandoffX`.

## Current status
- Zone 9 is the only selectable map; Province and other maps are not shown.
- The menu has mode groups inspired by the new Standoff 2 interface: General (Team Fight, Allies) and Others (Training).
- Mode selection is saved locally in the browser. At this stage the buttons select a mode for the prototype UI; online matchmaking and full Team Fight/Allies rules are not connected in this repository yet.
- Settings are opened/closed from the top-right gear; the menu is responsive on mobile.
- The placeholder procedural knife has been removed because it did not meet the requested visual quality.
- A proper knife animation can be integrated after the matching Unity animation, rig/model and hand/weapon assets are supplied. A `.anim` file alone may not be sufficient if its bone paths or Avatar refer to a specific rig.

## Match HUD and pause
- Added a compact grayscale HUD with team labels / score, round timer, health, armor, weapon and ammo indicators, and an icon-only pause button.
- `Esc` opens the in-match pause screen. Resume returns to the first-person view; `Back to menu` brings back the lobby.
- The pause screen includes CT / T selection, HUD scale and opacity, HUD visibility presets, crosshair shape, three layout presets, graphics quality, sensitivity, and a draggable HUD editor with saved positions.
- HUD settings and team choice are stored locally in the browser. CT/T currently changes the prototype's local selection and team labels; there is no authoritative team system in a game server.
- Mobile displays monochrome touch controls and supports touch-look / movement as a basic prototype.

## Controls
- WASD / arrow keys: walk
- Mouse (desktop) / touch drag (mobile): look around
- Space: jump
- Shift: run
- N or the Noclip button: fly through walls; Space/Ctrl up/down
- G: show/hide the developer position panel
- Esc: pause / match settings
- X/Y/Z coordinates: numeric fields and sliders
- Settings include player size and movement-speed sliders

## GitHub Pages
Keep `index.html`, `zone9_explorer.html`, and `zone9.glb` in the repository root. Enable Pages from `main` / root in **Settings → Pages**.

Expected URL: https://standoffx.github.io/zone9prototype/

## Zone 9 GLB
The page loads `zone9.glb` from the direct GitHub Raw URL `https://raw.githubusercontent.com/standoffX/zone9prototype/main/zone9.glb`. If the Raw download fails, it retries `./zone9.glb` from the same site. The model currently stored in this repository is about 56 MB, so the first load may take time on a slow connection.

## Prototype boundaries
This repository currently contains a first-person map explorer, not a complete online shooter. The health, armor, ammo and score in the HUD are illustrative UI values; there is no weapon firing, damage, round logic, live scoreboard or server-backed team switching yet. The lobby mode buttons are still local selections. Those gameplay systems need to be implemented before the page can host real matches with other players.
