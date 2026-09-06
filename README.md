# D's Rent Tracker V1.8 — Data Safe

GitHub Pages-ready iPhone-first rent tracker.

## Data protection
- Keeps the existing `rentTrackerV1Data` storage key.
- Loads existing valid data before creating defaults.
- Never initializes default data over an existing valid record.
- Adds schema normalization/migration for future updates.
- Keeps a separate last-known-good internal backup in Local Storage before replacing the primary record.
- Adds **Backup data** to download a complete JSON backup.
- Adds **Restore data** to restore a JSON backup.
- Adds **Export data** and **Verify data**.
- Existing house/payment data remains intact when moving from V1.7 to V1.8.

## Payment correction
- History supports editing payment amount/month/date.
- History supports deleting an individual payment.
- Houses are never deleted by the payment controls.

## Important
Local Storage is still browser-managed. A downloaded backup file is the safest independent copy. Do not clear Safari website data before creating a backup.

## Deploy
Replace the files in the GitHub repository root and redeploy GitHub Pages. Keep the same site/domain.
