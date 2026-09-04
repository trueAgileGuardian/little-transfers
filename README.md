# Little Transfers v2

A phone-first transfer habit tracker.

## V2 changes
- Separates mandatory **BILLS** (Bills, Car loan, Insurance, Phone) from discretionary **GOALS** (House, Family, Travel, Piggy Bank).
- Adds **Piggy Bank** as a flexible future-spending savings bucket with no required target.
- Adds a second **Spend vs Save** page.
- Credit-card payments are entered as actual custom amounts per paycheck.
- Spend vs Save compares credit-card payments against GOALS only; mandatory bills are excluded.
- Replaces “planned baseline” wording with “left to transfer this month.”
- Keeps Check 1 / Check 2 and optional Check 3 behavior.
- Migrates existing v1 browser data automatically when opened on the same GitHub Pages URL.

## Updating GitHub Pages
Upload/replace `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`, and `README.md` in the repository root. Keep the same GitHub Pages URL so the browser can retain and migrate the existing local data.

Data is still stored locally in the browser. Clearing Safari website data can erase it.
