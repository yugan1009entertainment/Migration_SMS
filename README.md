# Suresh Migration Studio

Tableau → Power BI migration tool. Single-file, fully client-side application.

Copyright (c) 2026 Suresh Mani. All rights reserved. Proprietary and confidential.

## Architecture

- Static single-page app — `public/index.html`
- No build step, no server, no external network requests
- Fonts embedded as base64; React and JSZip bundled inline
- State persisted in browser `localStorage` / `indexedDB` (nothing leaves the device)

## Local preview

    npx serve public

Then open the printed localhost URL.

## Deploy (Vercel)

Framework Preset: **Other**
Build Command: *(leave empty)*
Output Directory: `public`
Install Command: *(leave empty)*

Vercel serves `public/index.html` at `/` automatically.
