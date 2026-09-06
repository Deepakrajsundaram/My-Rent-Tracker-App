# D's Rent Tracker V1.2

GitHub Pages-ready, iPhone-first rent tracker.

## Files
- `index.html` — application
- `ds_rent_tracker_logo.png` — master logo
- `apple-touch-icon.png` — iPhone Home Screen icon
- `manifest.json` — web app metadata
- `README.md` — setup notes

## GitHub Pages
Put all files in the repository root on the `main` branch, then use:
Settings → Pages → Deploy from a branch → `main` → `/(root)`.

## V1.2 changes
- D's Rent Tracker favicon
- iPhone Home Screen icon
- PWA manifest
- Fixed local month/date handling
- History screen
- Last-month pending amount on dashboard
- Payment month selector
- Previous unpaid months can be selected when recording a payment
- Existing localStorage key/data structure preserved

## Data preservation
The app uses the existing `rentTrackerV1Data` localStorage key.
Do not change this key in future versions. Future versions should migrate
existing data instead of clearing or replacing it.

## Important
GitHub Pages hosts the app code but does not synchronize localStorage
between devices. Data remains local to the browser/device.
