# Zone 9 Explorer v4

Standalone browser map explorer for `zone9.glb`. This is a separate project and does not modify StandoffX.

## Controls
- WASD / arrow keys: move
- Mouse: look around
- Space: jump
- Shift: run
- N or the Noclip button: toggle flying through walls
- In Noclip: Space rises, Ctrl descends
- G: hide/show the control panel
- X/Y/Z numeric fields and sliders: teleport/set coordinates
- The panel also includes player-size and movement-speed sliders

## GitHub Pages
The Pages entry point is `index.html`, which opens `zone9_explorer.html`. For automatic map loading, put `zone9.glb` at the repository root next to both HTML files. If it is absent, use the file picker shown by the page.

To publish: repository **Settings → Pages → Deploy from a branch → main → /(root) → Save**. Expected site URL: https://standoffX.github.io/zone9prototype/.

Note: the GLB asset is not stored in this commit; add your local `zone9.glb` file to the repository root and commit it separately. The file is about 54 MB, so use git from your computer instead of the small-file editor if GitHub's web uploader rejects it.
