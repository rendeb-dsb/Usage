Usage PWA - b1v9

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

Timer: Start/Stop displays elapsed time as m:ss.mmm and updates smoothly. Duration receives only m:ss (whole seconds), never milliseconds. Timer starts at 0:00.000 and is limited to 9:59.999. The Time entry field follows the current clock while it is untouched and no saved record is selected; manually edited times are preserved.

Update: The + button resets the timer to zero. The +5 and -5 duration adjustment controls and logic have been removed. Start/Stop and the millisecond timer are centered in the space between Duration and Med.


List views: Detail view includes the calculated Count and two-letter Day columns. Summary view groups records by date and displays the number of records, Day, Date, Med (the most recent Med value for that date), average Duration, and average Last Diff between consecutive records on that date.


Build b1v9 changes:
- Detail view columns shifted left: Date 35 px, Time 20 px, Duration and Last Diff 10 px.
- Timer Start/Stop button shifted 5 px right; timer display shifted 5 px left.
- The header above the detail Count column shows the sum of all displayed per-record counts.
- Summary view Count header shows the total number of records represented; Date, Med, Avg. Dur., and Avg Last Diff columns shifted left by the requested amounts.
- Settings includes JSON Export and Import. Export saves the complete SQLite database in a JSON file. Import validates the backup format and Usage table columns, asks for confirmation, then replaces the current local database.
