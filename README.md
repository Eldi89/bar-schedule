# Behind the Bar

Weekly schedule builder for a New York bar team (bartenders, barbacks, any role you add).
Single `index.html`, no build step, no server. Data stays on the device (localStorage), with backup and restore files.

## What it does

- **Day builder** (phone) and **week grid** (desktop): tap an open spot, pick from a ranked list of who can work it.
- **Auto-fill**: fills open spots from your staffing targets. Respects availability, time off, max hours, rest between days and a day off each week, and spreads busy-night shifts evenly. Hand-placed shifts are never touched.
- **NY checks**: overtime after 40h, spread of hours (12 NYCRR 146-1.6), meal breaks (Labor Law §162), day of rest (Labor Law §161), double bookings, time off conflicts, understaffed shifts.
- **Labor estimate**: wages before tips with the NYC 2026 tip credit, tipped overtime rate, spread of hours pay, and labor % against a sales forecast.
- **Sharing**: picture for the group chat, plain text, a read-only staff link (each person picks their name and adds shifts to their calendar), .ics calendar files, print or PDF.
- Undo for every change, copy last week, mark a week as sent and flag later edits.

## Deploy

1. Import this repo in Vercel (framework preset: Other, no build command, output directory: root).
2. Open the Vercel URL on the iPhone in Safari, tap Share, then Add to Home Screen.

Every push to `main` redeploys automatically.

## Files

- `index.html` the whole app
- `manifest.json`, `icon-180.png`, `icon-512.png` Home Screen install

Pay figures and rules are editable in Setup. A scheduling aid, not legal advice.
