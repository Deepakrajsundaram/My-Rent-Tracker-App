# D's Rent Tracker V1.9

## Deployment
Replace the old GitHub Pages files with `index.html` and `manifest.json`.

## Critical data compatibility
- The app keeps the existing Local Storage key: `rentTrackerV1Data`.
- Existing V1.8 browser data is intended to load automatically.
- Do **not** clear browser/site data.
- If V1.8 still opens, use **Settings → Backup data** before replacement.

## Backup features included
- Backup data: downloads a complete JSON backup.
- Restore data: restores a JSON backup.
- Export data: downloads the current data as JSON.
- Verify data: checks whether stored data is readable.
- Internal last-known-good backup is stored under `rentTrackerV1DataBackup`.

## Main V1.9 fix
The V1.8 source contained a duplicate `let editPaymentId` declaration, which causes a JavaScript SyntaxError and prevents the whole app from initializing. V1.9 removes that duplicate declaration while keeping the existing storage key and data format.
