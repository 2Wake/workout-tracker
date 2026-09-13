# Gym Log & Tracker

A self-contained, phone-friendly workout tracker for a rehab-aware strength routine
(built around ACL/knee recovery and lower-back care). It runs entirely in the browser —
no account, no server, no data leaving your device.

## What's in here

| File | What it is |
| --- | --- |
| `index.html` | **The tracker** — log weights, check off exercises, see weekly progress. This is the main page. |
| `gym-log.html` | A simpler, printable gym log (day tabs, checkboxes, no saving). |

## Features (the tracker)

- **Day tabs** — an Upper/Lower rotation across 5 days; open just the day you're training.
- **Log as you go** — a field on every exercise for weight/reps/notes; entries auto-save while you type.
- **Save session** — files the day into your history with a timestamp.
- **"Last: …"** — each exercise shows what you did last time, so you know the number to beat.
- **This Week tab** — sessions this week, day types trained, and a per-exercise trend
  (**▲ up / ▼ down / = / new**) comparing your latest number to the previous one.
- **Export / Import backup** — download all your data as a `.json` file and restore it anytime.
- **PT / SKILL tags** — flags prescribed rehab exercises and skill movements (e.g. Turkish get-ups).
- **Print** — prints the full plan (or blank copies for pen logging).

## How to use

1. Open `index.html` in your browser (see hosting note below for reliable saving).
2. Pick a day, do the workout, and type your **top weight** into each exercise box.
   The trend reads the first number, so `155 x 8` is tracked as `155`.
3. Tap **Save session** when you finish the day.
4. Check the **This Week** tab for your summary, and **History** for past sessions.

> Detailed set-by-set logging can live in another app (e.g. Garmin); the tracker only
> needs the top number per exercise for its trend view.

## Hosting (GitHub Pages)

This site is static, so GitHub Pages serves it for free:

1. Put these files in a public repository (with `index.html` at the root).
2. **Settings → Pages →** Branch: `main`, Folder: `/ (root)` → **Save**.
3. After a minute, your site is live at:
   ```
   https://<your-username>.github.io/<your-repo>/
   ```
4. Open that link in **Safari** (iPhone) → **Share → Add to Home Screen** for an app-like icon.

To update later, upload the new file with the same name — the link stays the same.

## Where your data lives

- Logged sessions are stored in your browser's **local storage**, on the device you use —
  they are **never uploaded** to GitHub or anywhere else.
- Storage is tied to one browser on one device. Use one "home base" device for logging.
- Saving works reliably when the page is opened from a **real web link** (hosted), not as a
  local file. If a warning bar appears at the top, saving is off — host it or open it directly.
- Clearing your browser data erases the log, so **Export a backup every week or two.**

## A note on safety

This is a personal training aid, not medical advice. It assumes an active rehab plan
supervised by a physical therapist. The general rules baked into the plan:

- **Watch your legs** — stop any movement that sends pain/tingling/numbness down the leg.
- **Knee** — familiar donor-site tenderness that warms up is usually OK; sharp, deep, or
  joint-line pain should be flagged, not pushed through.
- Run loads, ranges, and progressions past your PT.
