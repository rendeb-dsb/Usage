Usage PWA - b1v5

Files:
- index.html: application
- manifest.webmanifest: PWA metadata
- sw.js: service worker

Database:
- SQLite database name: ManageDB (SQLite database stored as bytes in this browser's IndexedDB persistence container)
- Table: Usage
- Fields: ID, Med, Date, Time, Duration

Notes:
- First load requires an internet connection to load sql.js from cdnjs. Once loaded, the SQLite database is persisted locally on this device.
- Host the folder contents on HTTPS (for example GitHub Pages) to install as a PWA.
- Data is local to this browser/device; it is not synchronized to other devices.

Timer: Start/Stop control advances once per second and continuously copies its m:ss value into Duration. Timer starts at 0:00 and is limited to 9:59 to match the Duration field format.
