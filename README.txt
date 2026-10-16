# Avengers: Doomsday Savings PWA

## What's included
- `index.html`: the savings tracker
- `manifest.webmanifest`: install/app metadata
- `service-worker.js`: offline cache
- PNG app icons

## Important
A PWA must be served from HTTPS (or localhost) to install and use its service worker. Opening `index.html` directly as a local file will not enable full PWA installation/offline caching.

## Publish using GitHub Pages
1. Sign in to GitHub and create a new public repository.
2. Upload all files in this folder to the repository root (not the ZIP itself).
3. In the repository, open Settings → Pages.
4. Under Build and deployment, select Deploy from a branch; choose `main` and `/(root)`, then Save.
5. Wait for GitHub Pages to publish and open the URL it shows. It usually looks like `https://YOUR-USERNAME.github.io/REPOSITORY/`.
6. In Chrome on Android, open that URL, tap the three-dot menu, then choose “Install app” or “Add to Home screen” (wording varies).

## Transfer balance from the old local HTML
The old file and the hosted PWA have separate browser storage. Open the old tracker, note the displayed balance, then open the PWA and tap “نقل رصيد من النسخة القديمة”, enter that amount, and confirm. This copies the number manually; it cannot automatically read data from the local file.

## Privacy
The tracker saves the balance in browser storage on your device. It is not a bank account and does not sync across devices. Clearing site data can erase the saved progress.
