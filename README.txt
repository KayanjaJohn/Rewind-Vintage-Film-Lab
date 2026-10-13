REWIND — Vintage Film Lab PWA

CONTENTS
- index.html: app, image processing, custom presets, added film looks and texture styles
- manifest.json: PWA install metadata
- sw.js: service worker for offline app-shell caching
- icon.svg: app icon

INSTALL
A PWA cannot reliably install from a standalone file:// HTML file. Deploy ALL files in this folder to the same HTTPS website (or run on localhost). Then open the site in a supported browser, such as Android Chrome, and choose the browser menu > Install app / Add to Home screen.

HOSTING
Upload these files, preserving their names, to a static HTTPS host such as GitHub Pages, Netlify, or Vercel. No build step is required.

NOTES
- Photo transformations run in the browser; photos are not uploaded.
- Custom presets are saved in localStorage on that browser/device.
- Offline app-shell caching is enabled after the first successful visit online.
- Some browser/PWA validators may require PNG icons at 192x192 and 512x512; SVG icons work in modern browsers.
