# Daily Fuel — meal, protein, water & budget tracker

## What's included
- `index.html` — mobile-first app with Today, Activity, and Settings.
- `manifest.json`, `service-worker.js`, `icon.svg` — installable PWA support.
- Local IndexedDB storage for daily records and settings.
- Activity dashboard with protein/water trend charts, goal consistency, streaks, summaries, and saved day details.
- JSON export/import backups.
- Daily motivational/reflection quote: shown once per day in a popup, then kept below the Today hero; refresh for another quote. It tries the free Quotable API and uses built-in quotes when the API is unavailable. Quotes are stored locally in the browser.

## Run locally
Use a local static server, for example:
```bash
python -m http.server 8000
```
Then open `http://localhost:8000` on the device/browser. For installation on a phone, host the folder over HTTPS and use the browser's **Install app** / **Add to Home Screen** option.

Opening `index.html` directly is suitable for a quick preview, but PWA service workers generally require HTTPS or localhost.

## Data and privacy
App data is stored in the browser's IndexedDB database on that device. Browser storage can still be cleared or evicted, so export a JSON backup regularly. The app does not send your tracker data to a server.

## Notes
Protein amounts are editable estimates, not laboratory measurements. Weight-based protein and water calculations are general estimates; adjust to your needs and seek individual medical advice if a health condition affects nutrition or fluid intake.
