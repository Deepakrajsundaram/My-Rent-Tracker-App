# D's Rent Tracker V1.4

GitHub Pages-ready iPhone-first rent tracker.

## V1.4
- Fixed Settings scrolling so all 6 houses are accessible.
- Fixed History navigation with a clear back-to-home button.
- Added direct Edit House screen.
- Tapping a house card still records a payment; editing is done from Settings/Manage.
- Payment month can be selected, including older months with outstanding rent.
- Last-month pending amount shown on the dashboard.
- Share status includes all active houses, current payment status, and payment date/amount details.
- Added versioned, uniquely named iPhone icons to prevent the old To-Do icon from being reused by Safari cache.
- Added the D's Rent Tracker logo inside the app header.
- Preserves the existing `rentTrackerV1Data` localStorage key and existing payment data.

## GitHub Pages
Put all files in the repository root on `main`, then deploy:
Settings -> Pages -> Deploy from a branch -> main -> /(root).

## Important for the iPhone icon
After deployment, delete the old Rent Tracker Home Screen shortcut and add the site again from Safari:
Share -> Add to Home Screen.
The icon filenames are intentionally versioned/unique for this app.

## Data
Rent data is stored locally in the browser/device. GitHub Pages does not synchronize localStorage between devices.
