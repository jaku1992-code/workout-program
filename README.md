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

Also included: `benchamin-franklin-ii.csv` — a full 8-week, 3-day/week
bench-focused program ("BENCHamin Franklin II"), transcribed from a
handwritten template with deadlift moved from day 1 to day 2 every week. A
larger, real-world example of what a filled-out program looks like.

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

## Building a program in the app

No spreadsheet needed — tap the pencil icon (top right) to open the builder:

- **+ Add set** — copies your last row and bumps the set number. Use this
  for back-to-back top sets of the same lift.
- **+ New lift, same day** — starts a fresh lift on the same week/day.
- **+ New day, same week** / **+ New week** — jump ahead when you're done
  with the current day or week.
- Each row: week, day, set number, lift name, percent of 1RM (leave blank
  for bodyweight), reps, and an optional video link.
- **Load into tracker** — puts the program to use right away.
- **Download as CSV** — saves it as a file if you want a copy or want to
  upload it later.
- **Start from sample** — fills the builder with the sample program so you
  can see the shape and edit from there.

## Personalizing the look

Gear icon → Appearance: pick an accent color, a highlight color, and a font
pairing. Changes apply immediately and are saved with your data.
