# Field Book v0.0.2

Prototype deliberately redesigned from scratch around the physical survey field-book concept.

## Flow
1. Launch
2. Create New Job or Job Storage
3. Open a job
4. Full-screen digital field-book page
5. Add basic field notes

## Current scope
- Mobile-first PWA
- Local job storage
- Job numbers
- Full-page lined field-book view
- Basic field notes
- Minimal job details
- Offline service worker

The survey-specific field-book tools are intentionally not built yet. They will be designed from the field-book interface outward in later versions.


## v0.0.3 update system

The PWA update mechanism was strengthened for GitHub Pages/Home Screen use:
- HTML uses a network-first strategy.
- Service-worker registration uses `updateViaCache: none`.
- The app explicitly calls `registration.update()` when launched.
- Old Field Book caches are removed on activation.
- The page reloads automatically when a new service worker takes control.
