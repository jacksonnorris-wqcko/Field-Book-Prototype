# Field Book v0.0.14

## Field tools
- Selecting a tool automatically closes the tool tray.
- The field page opens with no drawing tool selected.
- Line is now a tap-to-tap polyline:
  - tap A
  - tap B to create A-B
  - tap C to create B-C
  - continue tapping
- Double-tap while drawing a polyline to add the final segment and close it back to the original starting point.
- Finish Line still lets you stop without closing.

## Update system
v0.0.13 had a service-worker install problem: its cache list still referenced an old `icon.svg` that no longer existed. That could prevent the new service worker from installing, which explains why the Home Screen version was not updating.

v0.0.14 fixes the cache list and adds a no-cache `version.json` release check. The app checks on launch and periodically while open, then activates/reloads the new service worker.

Files:
- index.html
- manifest.json
- sw.js
- version.json
- field-book-logo-v012.png
