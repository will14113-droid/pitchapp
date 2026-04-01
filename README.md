# Pitch Charter — PWA Setup Guide

A baseball pitch charting app that runs on your iPad home screen.

---

## Files
- `index.html` — the entire app
- `sw.js` — service worker (offline support)
- `manifest.json` — PWA config (makes it installable)

---

## How to get it on your iPad (free, ~10 minutes)

### Option A: GitHub Pages (recommended, free forever)

1. Go to https://github.com and create a free account if you don't have one
2. Click **New repository** — name it anything (e.g. `pitchapp`)
3. Set it to **Public**
4. Upload all three files: `index.html`, `sw.js`, `manifest.json`
5. Go to **Settings → Pages → Source** → select `main` branch → Save
6. GitHub gives you a URL like `https://yourusername.github.io/pitchapp`
7. Open that URL in **Safari on your iPad**
8. Tap the **Share button** (box with arrow) → **Add to Home Screen**
9. Done — it now lives on your home screen like a real app

### Option B: Netlify (even easier)

1. Go to https://netlify.com → sign up free
2. Drag the entire folder onto the Netlify dashboard
3. You get a URL instantly
4. Open in Safari on iPad → Share → Add to Home Screen

---

## How to use

**Setup screen:**
- Enter your team, the opposing team name, and the first pitcher's name
- Your game saves automatically — if you close and reopen, it picks up where you left off

**Chart view:**
- Tap the batter display to enter a jersey number (0–99)
- Select Fastball or Non-FB, then the result
- Tap anywhere on the strike zone to place the pitch
- "New AB +" starts a new at-bat for the same batter
- Use ‹ › arrows to switch between batters you've logged
- Use the pitcher tabs at the top to switch pitchers; + adds a new one

**Heatmap view:**
- Shows where the active pitcher has been throwing — all pitches, FB only, or Non-FB only

**History view:**
- Shows every batter's full at-bat history with a mini zone diagram per AB
- Use this to see what happened last time a batter was up

---

## Data
Everything saves to your device automatically (localStorage). No account, no server, no cost.
