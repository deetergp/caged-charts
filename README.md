# Woodshed

Installable web app with guitar practice tools for learning the neck. Works offline after the first visit.

**Live site:** https://deetergp.github.io/guitar-woodshed/

## Tools
- **CAGED Scale Positions** (`caged/`) – the five CAGED positions for major, major pentatonic, natural, harmonic and melodic minor, and minor pentatonic scales in any key, with a notes/intervals toggle.
- **Fretboard Note Trainer** (`notes/`) – a blank neck from the open strings to fret 12. *Name the notes*: type each note name; wrong answers turn red, and Clear starts over. *Find the note*: the app picks a random note and you click every place it lives (or just on one string).

## Install
- **iPhone / iPad (Safari):** Share → Add to Home Screen
- **Android (Chrome):** menu → Install app
- **Mac / PC (Chrome or Edge):** install icon in the address bar

Open it once while online; after that it works offline.

## Files
- `index.html` – home page linking to each tool
- `caged/index.html` – CAGED charts
- `notes/index.html` – note trainer
- `manifest.webmanifest` – app name, icons, display mode
- `sw.js` – service worker that caches everything for offline use
- `icons/` – app icons

## Adding a tool
Make a new folder with an `index.html` (copy the `← Woodshed` link, manifest/icon tags and service-worker registration from an existing tool), add a card for it on the home page, and add its paths to `CORE` in `sw.js`.

## Updating
After changing any file, bump `VERSION` in `sw.js` (e.g. `woodshed-v2` → `woodshed-v3`) so installed copies pick up the new version on their next launch or two.
