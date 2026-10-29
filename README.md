# Zone 9 Prototype — Lobby + Map Explorer

Standalone Zone 9 first-person prototype with a Standoff 2 Remastered-inspired lobby/mode selector. This is a separate project and does not modify `standoffX/StandoffX`.

## Current status
- Zone 9 is the only selectable map; Province and other maps are not shown.
- The menu has mode groups inspired by the new Standoff 2 interface: General (Team Fight, Allies) and Others (Training).
- Mode selection is saved locally in the browser. At this stage the buttons select a mode for the prototype UI; online matchmaking and full Team Fight/Allies rules are not connected in this repository yet.
- Settings are opened/closed from the top-right gear; the menu is responsive on mobile.
- The placeholder procedural knife has been removed because it did not meet the requested visual quality.
- A proper knife animation can be integrated after the matching Unity animation, rig/model and hand/weapon assets are supplied. A `.anim` file alone may not be sufficient if its bone paths or Avatar refer to a specific rig.

## Controls
- WASD / arrow keys: walk
- Mouse: look around
- Space: jump
- Shift: run
- N or the Noclip button: fly through walls; Space/Ctrl up/down
- G: show/hide settings
- X/Y/Z coordinates: numeric fields and sliders
- Settings include player size and movement-speed sliders

## GitHub Pages
Keep `index.html`, `zone9_explorer.html`, and `zone9.glb` in the repository root. Enable Pages from `main` / root in **Settings → Pages**.

Expected URL: https://standoffx.github.io/zone9prototype/

## Zone 9 GLB
The GitHub text-file integration used to edit the page cannot upload binary GLB models directly. Use the `Publish_Zone9_To_GitHub_Windows.bat` or `Publish_Zone9_To_GitHub_Mac.command` in the full ZIP to copy `zone9.glb` and the updated page into a local clone and push them to GitHub.
