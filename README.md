# D's Rent Tracker V2.0

## Fixed house order
1. Periyar St Lower
2. Periyar St Upper
3. K.N.P Back House
4. K.N.P Upper
5. K.N.P Front House
6. SPK Nagar Lower

## Data safety
- Preserves the existing `rentTrackerV1Data` storage key for backward compatibility.
- House names are hardcoded and cannot be edited in the UI. Tenant and rent remain editable.
- Uses schema versioning and normalization for future migrations.
- Creates two rotating internal backups before a write.
- Never replaces a corrupt existing primary record with a fresh empty dataset.
- Backup / Restore / Export / Verify are included.
- Restore backs up the current data first.
- Rendering does not write to storage; only actual data changes do.

## GitHub Pages deployment
Replace the old `index.html` and `manifest.json` with the files in this package. Do not clear browser/site data.

## Important
Before major future app replacements, use Settings -> Backup data and keep the JSON file in iCloud Drive/Files.
