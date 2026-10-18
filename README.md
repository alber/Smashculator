# Smashculator

A tiny step-by-step damage calculator for the Red Hulk loop in Magic: The Gathering.
One self-contained page, no dependencies, works offline once installed.

## Install on iPhone

1. Open the GitHub Pages address in **Safari**.
2. Tap **Share**, then **Add to Home Screen**.
3. Launch it from the icon. After the first launch it works in airplane mode.

## Updating

Edit `index.html`, commit and push. The phone picks up the new version on the
launch after it has been online. If you add or rename files, also update the
list in `sw.js` and bump its `VERSION`.

## Adding a card

Add an entry to `CARDS` near the top of the script in `index.html`, copying an
existing reflector (`onDamaged: reflect`). Only cards whose damage truly comes
back to Creature 1 belong there.

## Files

- `index.html`: the whole app (HTML, CSS, JS, embedded fonts)
- `manifest.webmanifest`: app name, icon and landscape orientation
- `sw.js`: service worker that caches the app for offline use
- `icons/`: home-screen and favicon icons

Fonts: Anton and IBM Plex Sans Condensed, SIL Open Font License.
