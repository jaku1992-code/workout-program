# workout-program

A workout tracker that runs entirely off a CSV file.

**How it works:**
- Open `index.html` in a browser (phone or desktop).
- Tap the gear icon, then upload a CSV that describes your program.
- The app calculates weights from your 1-rep maxes and displays your sets for
  each week/day.
- Type in what you actually lifted — it saves automatically and shows up in
  History.

## CSV format

One row per set. Header row required, columns in any order:

| column | required | meaning |
|---|---|---|
| `week`  | yes | week number (1, 2, 3, ...) |
| `day`   | yes | day number within that week |
| `lift`  | yes | exercise name, e.g. `Squat`, `Ab Wheel` |
| `order` | no  | set order within that lift/day (defaults to file order) |
| `pct`   | no  | percent of 1RM for that set. Leave blank for bodyweight/accessory work |
| `reps`  | yes | reps prescribed, e.g. `5`. End with `+` (e.g. `5+`) to mark a max-rep/AMRAP set |
| `video` | no  | a YouTube (or Vimeo) link for that lift. Shows a "Watch demo" button on the card |

A starter file is included: `sample-program.csv`. Open it in Excel, edit it
to match your own program, save as CSV, and upload it in Settings.

Settings also has a "Download sample CSV" button if you want a fresh copy.

## Backing up your progress

Your maxes, logged sets, and program are saved automatically in this browser
— but only in this browser, on this device. If you lose your phone or clear
its browser data, that's gone unless you've backed up.

- Gear icon → Backup → **Download backup file**. Save it somewhere off the
  phone (email it to yourself, a cloud drive folder).
- The app will remind you with a banner if it's been 14+ days since your
  last backup.
- To restore on a new phone or after wiping data: gear icon → Backup →
  **Restore from file**, and pick the backup file you saved.

## Personalizing the look

Gear icon → Appearance: pick an accent color, a highlight color, and a font
pairing. Changes apply immediately and are saved with your data.
