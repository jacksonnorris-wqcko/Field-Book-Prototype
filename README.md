# Field Book v0.0.4

Premium visual redesign of the digital survey field-book prototype.

The physical field-book concept remains the core interaction, but the interface has been rebuilt with a restrained professional aesthetic: dark field-book cover, sage/charcoal controls, warm paper, subtle ruled lines, brass accent and monospaced field-note typography.

## Flow
Launch → Create New Job / Job Storage → Open Job → Full field-book page.

Survey-specific tools remain intentionally minimal so they can be designed around the field-book surface in the next versions.


## v0.0.4 update behaviour

The service worker has been rebuilt to make GitHub Pages updates reliable for installed PWAs:
- `updateViaCache: none` forces the browser to check the service-worker script.
- `registration.update()` runs when the app opens.
- Navigation requests use `cache: no-store`, so the latest `index.html` is fetched from GitHub.
- New service workers activate immediately.
- Old caches are deleted during activation.
- The page reloads automatically when the new worker takes control.

After uploading v0.0.4 to GitHub Pages, close the installed Field Book app completely and open it once. From then on, future refreshes/openings should pick up new GitHub versions without requiring the user to clear Safari data.
