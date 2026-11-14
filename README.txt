Usage PWA - Build 1 Version 15
Displayed application version: b1v15

Data Entry layout updates from b1v12:
- Date calendar control reduced by an additional 20px (now 102px wide).
- Time textbox reduced by an additional 25px (now 85px wide).
- Med label and textbox remain on the first entry line, immediately to the right of the Time control set.
- Start/Stop button moved 30px to the right from its b1v12 position.

The timer continues to write elapsed m:ss directly into Duration. Existing SQLite ManageDB / Usage schema and local IndexedDB storage key are unchanged.

Data Entry layout updates from b1v13:
- Date calendar control widened by 20px (122px total).
- Time control set shifted 40px to the right from its previous visual position.
- Time textbox narrowed by 40px (45px total), reclaiming space on its right while the Med control remains right-anchored in its existing space.


Build 1 Version 15 changes:
- Time control set shifted 10px left; textbox widened 20px (65px total); 10px reduced from gap to Med label.
- Start/Stop button shifted 20px right (30px relative offset).
- Pressing Stop now stops the timer and invokes Add to save the current entry automatically.
- Detail list column order changed to Med, Last Diff, Duration.
- Roll-up Date column shifted 50px left and Count column shifted 250px left.

Build b1v16: Time field +10px; Roll-up Count +50px; Detail radio, count, and Time columns each narrowed 10px, shifting subsequent columns left; added small Data Entry change instructions.
