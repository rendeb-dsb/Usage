Usage PWA - Build 1 Version 10
Displayed application version: b1v10

Changes in b1v10:
- Duration entry width reduced by 25%.
- Med entry width reduced by 50%; Med label and field are right-justified.
- Timer display shows m:ss without thousandths; elapsed precision remains internal.
- Day column moved 5px toward Date.
- Data Entry and Last Used panels remain sticky together at the top while the Data List has its own vertical and horizontal scrolling area.
- Detail header count is the number of detail rows (records), not the sum of the per-day sequence values.
- Summary header count is the number of summary rows (dates), not the sum of daily record counts. Summary columns now align with their data; no extra empty column is present.

Database:
- SQLite database ManageDB, table Usage.
- Local database persistence remains in IndexedDB under UsageLocalStore / usage-managedb-sqlite-v1.
- Import and Export JSON database backup remain available on Settings.
