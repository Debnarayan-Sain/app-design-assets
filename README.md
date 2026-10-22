# App Design Assets

Central asset repository for the telecom dealer app UI.

## Structure

- `assets/icons/` — reusable UI icons, preferably SVG
- `assets/illustrations/` — telecom towers, route maps, wallet art, and other decorative visuals
- `assets/backgrounds/` — screen and card background artwork
- `assets/themes/` — theme tokens and theme-aware usage guidance
- `asset-manifest.json` — machine-readable asset index for Claude and other tooling

## Recommended formats

- SVG for icons and theme-aware illustrations
- WebP for raster artwork and textured backgrounds
- PNG only when transparency or source compatibility requires it

## Theme-aware assets

Where possible, keep SVG geometry shared and make colors configurable through `currentColor`, CSS variables, or component props. The same asset should adapt to Light, Dark, Blue, and Green themes instead of duplicating artwork unnecessarily.

## Claude workflow

Claude can connect to this repository and use the exact assets from these paths rather than recreating them from screenshots.
