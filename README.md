[README.md](https://github.com/user-attachments/files/29181445/README.md)
# Air Force FIP Companion

A single-file web app for running and tracking a unit Fitness Improvement Plan:
workout checklists (4-week bodyweight cycle + 12-week program), a one-page
"Training Day" view with per-trainee circuit clocks, a progress logger
(weight, waist/WHtR, test components, steps, sleep, sessions, back-pain),
a HAMR mock-test beep timer, dark mode, and CSV/JSON export.

Everything is contained in **`index.html`** — no build step, no dependencies, works offline.
Data is stored in the browser (localStorage) on each device; use the **Data** tab to export/import JSON backups.

## Host on GitHub Pages

1. Create a new repository (e.g. `fip-companion`).
2. Upload **`index.html`** to the repository root (and this `README.md` if you like).
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
6. Wait ~1 minute; your app will be live at
   `https://<your-username>.github.io/<repo-name>/`

Open that URL on a phone and use the browser's **Add to Home Screen** to keep it one tap away on the field.

## Notes
- The HAMR timer uses the EuroFit 20m protocol (Level 1 = 8.0 km/h, +0.5/level). For an **officially scored** test, use your unit's certified audio.
- Audio needs a tap to start on mobile (browser autoplay rules) — press Start.
- Data does not sync between devices automatically; export JSON to move it.
