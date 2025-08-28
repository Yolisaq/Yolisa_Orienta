# Orienta — One‑Page Orientation Web App

**Features mapped to device orientation**

- **Portrait (upright, angle 0):** Alarm Clock (set/clear/snooze 5m)
- **Landscape right (angle 90):** Stopwatch (start/pause/reset)
- **Portrait upside down (angle 180):** Timer (set minutes/seconds; start/pause/reset)
- **Landscape left (angle 270):** Weather of the Day (Open‑Meteo; geolocation with Johannesburg fallback)

## Run locally
1. Download `index.html` and open it in a **mobile browser** (Android Chrome / iOS Safari). It also works in desktop with DevTools device toolbar.
2. Allow **Location** for weather, or tap **Use JHB**.
3. Rotate the device to switch features seamlessly.

> Tip (desktop): In Chrome, open DevTools → Toggle Device Toolbar → set a phone, then press `Ctrl/Cmd+Shift+P` → “Show device frame”, and rotate.

## Deploy (free)
**GitHub Pages**
1. Create a repo (e.g., `orienta`), upload `index.html` to the root.
2. Settings → Pages → **Deploy from branch** (main / root). Your URL will be `https://<username>.github.io/orienta/`.

**Netlify (drag & drop)**
1. Go to app.netlify.com → New site from Git → choose your repo, or drag‑drop a folder with `index.html`.
2. You’ll get a `https://<name>.netlify.app` URL.

## Tech notes
- Runs 100% in the browser (no backend).
- Orientation detection uses `screen.orientation.angle`, `window.orientation` (iOS fallback), and a resize fallback.
- Weather: [Open‑Meteo](https://open-meteo.com/) — free, no API key. We request `current_weather` and daily high/low.
- Works on Android and iOS. On iOS, upside‑down may be disabled by system in some apps, but Safari allows it.

## Demo video (≤ 2 min) — suggested script
1. **Intro (10s):** “This is *Orienta*, a mobile‑first web app that changes tools when you rotate your phone.”
2. **Portrait ↑ Alarm (20s):** Show clock; set alarm for 1 minute; mention snooze; quick ring preview.
3. **Landscape → Stopwatch (20s):** Start, pause, resume, reset.
4. **Portrait ↓ Timer (20s):** Set 0 min 10 sec; start; show vibration/sound.
5. **Landscape ← Weather (25s):** Allow location; show temps and summary; tap **Use JHB** fallback; tap **Refresh**.
6. **Wrap (15s):** “All in one file, no backend. Open‑Meteo free API. Works on Android & iOS. Open‑source on GitHub Pages.”

Record on your phone (screen recorder), or on desktop using Chrome’s device emulator.

## Evaluation checklist
- **Functionality:** Four modes auto‑switch on orientation.
- **UX:** Big touch targets, clear labels, smooth fade transition, single‑screen controls.
- **Prompting:** See `prompts_used.md` for full AI prompting log.
- **Technical:** Clean, commented single‑file HTML/CSS/JS; resilient orientation detection; no dependencies.
- **Wow:** A complete multi‑tool utility in just one file with polished UI, vibration and sound cues.
