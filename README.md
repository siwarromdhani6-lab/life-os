# LIFE OS

A single-page personal life planner with a terminal/hacker aesthetic — built as an installable PWA. Runs entirely in the browser with no backend required.

![theme](https://img.shields.io/badge/style-Arch%20terminal-e5323c?style=flat-square) ![storage](https://img.shields.io/badge/storage-localStorage-c9a15a?style=flat-square)

## What it does

- **Neofetch-style dashboard** — an ASCII/terminal-inspired hero panel summarizing your day
- **Today / Week / Progress tabs** — plan events, see your week at a glance, and track completion stats and streaks
- **Events & notes** — add, complete, and manage daily events; keep freeform notes
- **Draggable "hacking sticker"** widget for a bit of terminal flavor
- **Installable PWA** — add to your home screen on mobile or desktop via the included manifest and icons
- **Optional cloud sync** — connect a [ntfy.sh](https://ntfy.sh) topic for push notifications and a Google Apps Script URL as a simple free backend to sync data across devices

## Storage

All data lives in the browser's `localStorage` by default — nothing is sent anywhere unless you explicitly configure the optional sync settings (ntfy topic + Apps Script URL) in the app.

## Running it

No build step, no dependencies — it's a static site.

- **Locally:** open `index.html` directly in a browser, or serve the folder with any static file server.
- **As an installable app:** serve it over HTTPS (see GitHub Pages below) and use "Add to Home Screen" / "Install App" in your browser.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The entire app — HTML, CSS, and JS in one file |
| `manifest.json` | PWA manifest (name, theme color, icons) |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | App icons |
| `favicon.ico` | Browser tab icon |

## Deploying on GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under **Source**, select the `main` branch and `/ (root)` folder, then **Save**
4. Your site will be live at `https://<username>.github.io/life-os/` within a minute or two
