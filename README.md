# Zone 9 Explorer v6

Standalone first-person map explorer for Zone 9. This is a separate project and does not modify StandoffX.

## Map status
- **Zone 9** is the only selectable map for now.
- The supplied `province.glb` currently has detached building geometry and missing ground sections in the inspected preview. It is intentionally removed from the playable map selector until it can be rebuilt. The original asset is not deleted from the user's local files.

## Controls
- WASD / arrow keys: walk
- Mouse: look around
- Space: jump
- Shift: run
- N or the Noclip button: fly through walls; Space/Ctrl up/down
- Left mouse: knife slash
- Right mouse: quick thrust
- F: inspect knife
- G: show/hide settings
- X/Y/Z coordinates: numeric fields and sliders
- Settings also include player-size and movement-speed sliders

## Knife
The page uses an original procedural first-person tactical knife and custom idle sway, slash, thrust, and inspect animations inspired by FPS handling. No game-extracted Standoff 2 model or animation files are bundled. For visual/motion reference, a community video shows the Standoff 2 knife animations: https://rutube.ru/video/0dc8057b3cd015eaa124bf3afc2f9bab/

## GitHub Pages
Keep `index.html`, `zone9_explorer.html`, and `zone9.glb` in the repository root. Enable Pages from `main` / root in **Settings → Pages**.

Expected URL: https://standoffx.github.io/zone9prototype/

## Publish the map binary
The GitHub app integration used for code changes cannot upload the binary GLB directly. The Explorer v6 ZIP includes `Publish_Zone9_To_GitHub_Windows.bat` and `Publish_Zone9_To_GitHub_Mac.command`. Run the script from the extracted folder to clone the repository, copy the optimized `zone9.glb` and updated HTML, then commit and push. Authenticate with GitHub if prompted.

The provided Zone 9 GLB was optimized for web delivery by converting opaque color textures to JPEG while preserving the transparent decal and mesh geometry (approximately 56 MB → 17 MB).
