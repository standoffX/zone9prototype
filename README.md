# Zone 9 Explorer v5

Standalone first-person map explorer. It is a separate project and does not modify StandoffX.

## Maps
The start screen lets you choose **Zone 9** or **Province**, then press **Play**. Put these files in the repository root for automatic loading:
- `zone9.glb`
- `province.glb`

If the files are not hosted next to the HTML page, the file picker can load a GLB from your device manually.

## Controls
- `W A S D` / arrow keys — move
- Mouse — look around
- `Space` — jump; in Noclip, fly up
- `Shift` — run
- `N` or the Noclip button — toggle flying through walls
- In Noclip, `Ctrl` — fly down
- `G` — show/hide player panel
- X/Y/Z can be set by typing coordinates or using the sliders
- Panel includes player-size and movement-speed sliders

## GitHub Pages
The repository includes `index.html`, `zone9_explorer.html`, and `.nojekyll`. To publish: repository **Settings → Pages → Deploy from a branch → main → /(root) → Save**.

Expected URL: https://standoffX.github.io/zone9prototype/

## Add the map files
The two GLB models are large binary files (about 54 MB and 65 MB). They have not been uploaded to GitHub by the text-file integration used to update this repository. Add both files to the repository root with GitHub Desktop or Git:
1. Clone `https://github.com/standoffX/zone9prototype.git`
2. Copy `zone9.glb` and `province.glb` into the cloned folder
3. Commit and push the two files

The app will try to load each map from `./zone9.glb` or `./province.glb` depending on your choice.
