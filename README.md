# CAGED Scale Positions

Installable web app with the five CAGED positions for the major, natural minor and minor pentatonic scales on 6-string guitar, in any key.

**Live site:** https://deetergp.github.io/caged-charts/

## Install
- **iPhone / iPad (Safari):** Share → Add to Home Screen
- **Android (Chrome):** menu → Install app
- **Mac / PC (Chrome or Edge):** install icon in the address bar

Open it once while online; after that it works offline.

## Files
- `index.html` – the app (charts, key picker, notes/intervals toggle)
- `manifest.webmanifest` – app name, icons, display mode
- `sw.js` – service worker that caches everything for offline use
- `icons/` – app icons

## Updating
After changing any file, bump `VERSION` in `sw.js` (e.g. `caged-v1` → `caged-v2`) so installed copies pick up the new version on their next launch or two.
