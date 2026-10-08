# Field Book v0.0.16

Bug-fix release for v0.0.15.

v0.0.15 contained a JavaScript syntax error in the tool help configuration: the `move` help entry was missing a comma before `eraser`. Because the browser could not parse the script, the entire application JavaScript stopped loading, which broke Create New Job and Job Storage as well as the drawing functions.

v0.0.16 fixes that syntax error and verifies the embedded JavaScript parses successfully.

No intended UI or drawing-function changes were made in this release.
