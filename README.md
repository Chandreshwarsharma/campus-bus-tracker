# 🚌 Real-Time Bus Tracker — Gorakhpur

A live bus tracking web app for Gorakhpur, India, with a Transparency & Semi-Opacity
(frosted glass) design.

**Features**
- 🗺️ Live street map of Gorakhpur with 3 routes and 13 real stops
  (Gorakhpur Junction, Golghar, DDU University, MMMUT, BRD Medical College,
  Gorakhnath Temple, Asuran Chowk, Nausad, Airport…)
- 🚌 6 buses moving live with speed, status and crowd levels
- ⏱️ Per-stop ETA predictions — switchable V1 (distance ÷ speed) and
  V2 (time-of-day traffic-aware) models
- 🔔 Arrival alerts (3 / 5 / 10 minutes), crowd reports, nearest-stop finder
- 📱 Driver mode — a phone's real GPS takes over a bus on the map
- 📊 Admin dashboard — on-time stats, arrivals-per-hour chart, fleet table,
  trip log with CSV download
- 🔐 Sign-in (student / driver / admin), light & dark glass themes, mobile friendly

**Tech:** single self-contained HTML file — Leaflet + OpenStreetMap-style tiles,
vanilla JS. No build step, no API keys.

## 🚀 Put it live with GitHub Pages (free)

**Option A — web upload (no git needed)**
1. Create a new repository on GitHub (e.g. `bus-tracker`), **public**.
2. Click **Add file → Upload files**, drag in `index.html`, then **Commit changes**.
3. Go to **Settings → Pages** → under *Build and deployment*, set Source to
   **Deploy from a branch**, Branch to **main** / **(root)**, Save.
4. After ~1 minute your site is live at `https://<your-username>.github.io/bus-tracker/`.

**Option B — git push**
```bash
git init
git add index.html README.md
git commit -m "Real-Time Bus Tracker for Gorakhpur"
git branch -M main
git remote add origin https://github.com/<your-username>/bus-tracker.git
git push -u origin main
```
Then enable Pages as in step 3 above.

## 📁 What's in this repo

| File | Purpose |
|---|---|
| `index.html` | The entire app — open it directly in a browser or serve it anywhere |
| `README.md` | This file |

> Note: the live map tiles load from the internet, so the page needs an
> internet connection. Driver GPS / location features need HTTPS (GitHub Pages
> provides this) or localhost.
