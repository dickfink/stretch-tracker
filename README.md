# Morning Stretch PWA

A guided morning stretch routine — timed, offline-ready, installable on iPhone.

## Files

|File           |Purpose                                   |
|---------------|------------------------------------------|
|`index.html`   |The entire app (single file)              |
|`manifest.json`|PWA manifest for installability           |
|`sw.js`        |Service worker for offline support        |
|`icon-192.png` |App icon (192×192) — **add this yourself**|
|`icon-512.png` |App icon (512×512) — **add this yourself**|

## Setup

### 1. Create icons

You need two PNG icons. The easiest option:

- Use [PWA Asset Generator](https://www.pwabuilder.com/imageGenerator) or any design tool
- A simple green circle or your own logo works fine
- Save as `icon-192.png` (192×192 px) and `icon-512.png` (512×512 px)

> **Tip:** Without icons, the app will still work — it just won’t show a nice icon on the home screen.

### 2. Deploy to GitHub Pages

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/YOUR_USERNAME/morning-stretch.git
git push -u origin main
```

Then in your GitHub repo → **Settings → Pages → Source: main branch / root folder**.

Your app will be live at `https://YOUR_USERNAME.github.io/stretch-tracker/`
e.g 'https://dickfink.github.io/stretch-tracker/`

### 3. Install on iPhone

1. Open the URL in **Safari** (must be Safari for iOS PWA install)
1. Tap the **Share** button (box with arrow)
1. Tap **“Add to Home Screen”**
1. Tap **“Add”**

The app will appear on your home screen and launch full-screen like a native app. It works offline after the first load.

## Stretches

1. **90/90 Hip Stretch** — 60 seconds each side
1. **World’s Greatest Stretch** — 5 reps each side
1. **Cat-Cow** — 10 reps
1. **Thoracic Rotation** — 8 reps each side
1. **Standing Hip Circles** — 10 each direction
1. **Doorway Chest Opener** — 30 seconds × 2 sets

## Features

- ⏱ Countdown timer with animated ring for timed holds
- 👆 Tap-to-count for rep-based stretches
- 🔔 Audio chime + vibration when a hold ends
- 📍 Progress dots + bar showing position in routine
- ⏸ Pause/resume for timer steps
- ← Back button to revisit previous step
- 📴 Fully offline after first visit
- 📱 Installable on iPhone via Safari → Add to Home Screen