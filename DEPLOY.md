# ObAnesth — Deployment Guide

## Files in this package
- `App.jsx` — the full app
- `main.jsx` — React entry point
- `index.html` — PWA-enabled HTML shell
- `manifest.json` — PWA manifest (icon, name, theme)
- `sw.js` — service worker (offline support)
- `vite.config.js` — build config
- `package.json` — dependencies
- `public/icons/` — place your app icons here (icon-192.png, icon-512.png)

## Step 1 — Set up your project on GitHub

1. Go to github.com and sign in
2. Click the **+** icon top right → **New repository**
3. Name it: `obanesth`
4. Set to **Private**
5. Click **Create repository**
6. On the next screen, click **uploading an existing file**
7. Upload ALL files from this package
8. Click **Commit changes**

## Step 2 — Deploy on Vercel

1. Go to vercel.com and sign in
2. Click **Add New → Project**
3. Click **Import** next to your `obanesth` GitHub repo
4. Under Framework Preset, select **Vite**
5. Click **Deploy**
6. Wait ~60 seconds — Vercel gives you a live URL like `obanesth.vercel.app`

## Step 3 — Test PWA on your phone

1. Open the Vercel URL in Safari (iPhone) or Chrome (Android)
2. iPhone: tap Share → **Add to Home Screen** → **Add**
3. Android: tap the menu → **Add to Home Screen**
4. The app icon appears on your home screen and opens full-screen

## Step 4 — Update content anytime

1. Edit `App.jsx` with Claude
2. Download the new file
3. Go to your GitHub repo → click `App.jsx` → click the pencil icon
4. Delete all content, paste new content, click **Commit changes**
5. Vercel auto-deploys in ~30 seconds

## App Store submission (next phase)
- Google Play: use Bubblewrap or PWA Builder (pwabuilder.com) — free tool
- Apple App Store: requires $99/year Apple Developer account
