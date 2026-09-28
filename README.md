# Greenhouse-Textures
A texture/animation tool for PVZ2ge

The first public beta. Custom art for PvZ2 Gardenless, on any plant, vanilla or modded.

## What it does
- **Repaint sheets.** Save a plant's sprite sheet, edit it in any image editor, and put it back on one plant or on everything that uses the sheet.
- **Still images and fit to rig.** Replace a plant with a single picture, or fit your art onto the plant's existing rig.
- **Animation maker.** Cut your art into pieces, then build and animate it with Geometry Dash style triggers: Move, Rotate, Scale, Alpha, Show, Hide and Picture, with easing, on a timeline.
- **Packet editor.** Design the whole seed packet, not just the plant: colour, background, border and plant, with your own images for the background and border. Designs save to a library you can reuse.
- **Undo in place.** Anything you apply can be taken off again without restarting.

## Works with any mod
- Art for a plant is saved into the mod that adds that plant, so players get it just by installing that mod.
- Everything else goes to a home pack you choose under **Keep new art in**. If only one pack has a `textures/` folder, it's picked for you.
- Mod makers can list their own animation clips (a heal, a reload) through `globalThis.GreenhouseActs`, and the animation maker offers them. See "For plant mod makers" in the README.

## Install
1. Unzip into GP-Next's `packs` folder as `GreenhouseTextures`.
2. Turn on experimental JS modding (GP-Next 1.4.2 or later) and reload patches.
3. In a level, press **Ctrl+Shift+T**.

## Known limits
- This is a beta. Keep copies of art you'd miss; it's all plain PNG and JSON.
- Packs have to be unzipped for their art to be read or written. A zipped pack's art falls back to localStorage.
- A pack that ships art needs `textures/saved/` and `textures/removed/` to already exist, since the game may not let the pack create folders.

If something breaks, open an issue and include the "rig check" line the panel shows.
