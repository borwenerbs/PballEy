# PickleScore PWA

This is an installable, offline-first web app package.

## Publish it once over HTTPS
A Progressive Web App must be served from HTTPS (or localhost). The files cannot be installed as a PWA directly from the iPhone Files app.

Easy hosting options:
- GitHub Pages
- Netlify (manual deploy)
- Cloudflare Pages

Upload the *contents* of this folder so `index.html` is at the site root. Do not rename `manifest.webmanifest` or `sw.js`.

## Install on iPhone
1. Open the published HTTPS address in Safari.
2. Tap Share.
3. Choose Add to Home Screen.
4. Name it PickleScore, then tap Add.
5. Open it once while online so the service worker can cache the app.
6. After that, launch it from the Home Screen. It should work offline.

## Data
Player records, match history and current match are stored in browser local storage on this device. Use Export backup regularly. Clearing Safari website data can erase local records.

## Package contents
- `index.html` — app
- `manifest.webmanifest` — install metadata
- `sw.js` — offline cache
- `icons/` — app icons
