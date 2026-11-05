# Little Wonder Wheels 2.0 — Magical Adventure

A child-friendly 3D browser game based on the working v1.0.2 prototype. Built with Three.js, no account, ads, or analytics.

## Play

Publish all files in this folder to the root of a GitHub Pages repository. The `index.html` file must be at the repository root. Open the HTTPS Pages URL in a modern browser. Internet is required to load Three.js from a CDN (with fallback).

## Controls

- **Ayo Main:** start the game.
- **Ride:** left/right on screen or arrow keys / A/D on desktop. The bicycle moves forward automatically by default. Use the bell button for a chime.
- **Build:** drag the brick tile from the tray and release to snap the next bridge section, or press **Place**. Three sections complete the bridge. This is an assisted drag-to-place interaction, not freeform block construction.
- **Paint:** choose a swatch and tap a flower, tree, or bridge block.
- **Wonder Book:** view 5 achievements and 3 adventures.
- **Petualangan:** cycle through Bibi bridge, Poppy garden (color 5 distinct plants), and Milo bicycle park (ride near Milo).
- **Settings:** toggle Indonesian voice instructions (uses browser speech synthesis if supported), visual effects, and easy ride; customize bicycle frame color; reset progress.

## Save compatibility

The game intentionally retains the `lww_proto_v1` localStorage key from v1.0.2 and adds new fields. Existing saves should load. Browser clearing site data or resetting progress deletes local progress.

## Test checklist

1. Ayo Main opens the world (desktop and Android).
2. Ride and steering work, with a following camera.
3. Build by dragging a brick or using Place; complete bridge.
4. Paint five distinct plants in Poppy's quest.
5. Ride near Milo to unlock the park achievement.
6. Wonder Book displays achievements and quests.
7. Reload and verify bridge, colors, quest and settings persist.
8. Test landscape Android Chrome and check touch targets / FPS.
9. Test with network unavailable after first load; CDN dependencies may still prevent fully offline use.

## Known limitations

- Three.js is loaded from a third-party CDN. Offline reliability is not guaranteed.
- Dragging a brick anywhere over the game places the next bridge segment; this is an assisted snap interaction, not true 3D free-placement.
- Indonesian speech depends on the device/browser voices and may not be available.
- Performance and touchscreen usability have not been validated on physical Android devices in this environment.
- This is a feature-rich web prototype, not a Play Store-ready commercial release.

## Development

All app code is in `index.html`. No build step is required. Use a local static server for testing (`python -m http.server 8000`), or GitHub Pages. `sw.js` handles PWA cache lifecycle. No personal data is transmitted by game logic.
