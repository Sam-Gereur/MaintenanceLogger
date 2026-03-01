# 🚗 Garage Log

A mobile-first vehicle maintenance tracker PWA. Log jobs, track costs, analyse your fleet — works fully offline once installed.

## Features

- 📋 Log maintenance records with date, mileage, cost, job type and notes
- 🚗 Track multiple vehicles with purchase price & date
- 📊 Analytics: spending breakdowns, sparklines, cost per km
- 🎨 6 colour themes + dark/light mode
- 📤 Export filtered records to CSV
- ✏️ Edit and delete records
- 📱 Installable as a PWA — works offline

---

## Deploy to GitHub Pages (step by step)

### 1. Create the repo

1. Go to [github.com/new](https://github.com/new)
2. Name it `garage-log` (or anything you like)
3. Set it to **Public**
4. Click **Create repository**

### 2. Upload the files

In the new repo, click **"uploading an existing file"** and drag in all these files/folders:

```
index.html
manifest.json
service-worker.js
favicon.ico
icons/
  icon-72x72.png
  icon-96x96.png
  icon-128x128.png
  icon-144x144.png
  icon-152x152.png
  icon-192x192.png
  icon-384x384.png
  icon-512x512.png
```

Click **Commit changes**.

### 3. Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Under **Source**, select `Deploy from a branch`
3. Choose `main` branch, `/ (root)` folder
4. Click **Save**

After ~1 minute your app will be live at:
```
https://YOUR-USERNAME.github.io/garage-log/
```

---

## Install on your phone

### iPhone (Safari)
1. Open the URL in **Safari**
2. Tap the **Share** button (box with arrow)
3. Tap **"Add to Home Screen"**
4. Tap **Add**

### Android (Chrome)
1. Open the URL in **Chrome**
2. Tap the **three-dot menu**
3. Tap **"Add to Home screen"** or **"Install app"**
4. Tap **Install**

The app will appear on your home screen with the Garage Log icon and run fullscreen like a native app. It also works offline after the first load.

---

## Local development

Just open `index.html` directly in your browser — no build step required. 

For PWA features (service worker, install prompt) you need to serve over HTTPS or localhost:
```bash
npx serve .
# or
python3 -m http.server 8080
```
Then visit `http://localhost:8080`.
