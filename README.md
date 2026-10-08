# Field Book v0.0.5

Premium mobile-first digital survey field book prototype.

## Files

- `index.html` — app
- `manifest.json` — PWA configuration
- `sw.js` — offline storage and automatic update system
- `icon.svg` — app icon
- `README.md` — setup notes

## GitHub Pages

Upload/replace all files in the repository with these files, then allow GitHub Pages a moment to publish.

Open the GitHub Pages address on the phone and add it to the Home Screen.

## Automatic updates

v0.0.5 uses:
- service-worker `updateViaCache: "none"`
- explicit `registration.update()`
- versioned service-worker cache
- deletion of old Field Book caches
- network-first navigation
- network-first app assets
- automatic activation of waiting workers
- automatic page reload after a new worker takes control

Future releases should bump the `VERSION` in `sw.js`, the `APP_VERSION` in `index.html`, and the visible version text.

## Data

This prototype stores jobs locally in the browser/device. Cloud sync and server integration are not yet implemented.
