# Zone 9 Explorer v7

Standalone first-person map explorer for Zone 9. This is a separate project and does not modify StandoffX.

## Current status
- Zone 9 is the only selectable map. Province is temporarily hidden until its geometry can be rebuilt.
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
