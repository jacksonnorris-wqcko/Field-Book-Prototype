# Field Book v0.0.20

Digital survey field book PWA.

## v0.0.20
- Correct visible app version updated to 0.0.20.
- Polished line construction and double-tap closing so zero-length duplicate segments are not created.
- Undo now fully resets active line construction state.
- Tool changes clear unfinished construction state without deleting completed geometry.
- Undo during an unfinished arc cancels the construction instead of deleting saved geometry.
- Opening a job starts with a clean, neutral tool state.
- Pointer-cancel handling no longer risks committing partial drawings.
- Existing zoom, logo, job storage and drawing tools retained.
