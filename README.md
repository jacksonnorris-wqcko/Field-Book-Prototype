# Field Book v0.0.18

Zoom bug-fix release.

v0.0.17 mixed zoom handling directly into the field-tool pointer handlers, which interfered with the drawing tools.

v0.0.18 starts from the last known working v0.0.16 tool implementation and adds zoom as a separate gesture layer.

### Zoom
- Browser/iOS page zoom disabled.
- Two-finger pinch zooms the entire field page.
- Single-finger input is passed directly to the existing field tools.
- 65%–300% zoom.
- Zoom controls appear when zoomed.
- 1:1 resets the view.
- Opening a job resets zoom.

### Tools
The v0.0.16 field tools are retained unchanged:
- polyline line tool
- double-tap close
- arc start/end/radius workflow
- text move/rotate
- eraser
- pen
