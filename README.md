# Field Book v0.0.6

Digital survey field-book prototype.

## v0.0.6 focus

The field page is now intentionally open and uncluttered.

A compact **Tools** control exposes:
- Pen / freehand
- Straight line
- Arc
- Text
- Eraser
- Undo
- Clear page

Drawings are stored with each local job.

## GitHub Pages

Replace the complete contents of the repository with these files, then allow GitHub Pages to publish.

Open the GitHub Pages address and add it to the Home Screen.

## Updates

The PWA uses:
- versioned service-worker caches
- `updateViaCache: "none"`
- explicit service-worker update checks
- network-first navigation
- old-cache cleanup
- automatic activation
- automatic reload after the new worker takes control

## Data

Jobs and field sketches are currently stored locally on the device/browser. Cloud sync is not yet implemented.
