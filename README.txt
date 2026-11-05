Usage PWA - b1v3

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
