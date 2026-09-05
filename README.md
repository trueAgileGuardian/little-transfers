# Little Transfers v3.1.1

A local-first, phone-friendly PWA for tracking manual transfers, savings habits, and current-income spending.

## v3.0 — Profiles & Custom Setup
- Multi-profile support for Rachel and Matthew.
- Profile picker with user-chosen emoji/avatar and remembered last profile.
- Full read-only 👀 peek into the other profile.
- First-time setup wizard; Matthew can start blank or copy Rachel's setup.
- Configurable Bills, Goals, and flexible/no-target goals.
- Per-paycheck, per-month, and flexible target cadences.
- Optional third-paycheck contribution behavior for per-check goals.
- Goal emoji modes: Auto, Custom, or None.
- Manage Goals screen with forward-only target edits; historical entries retain goal snapshots.
- Separate contribution, Spend vs Save, card-payment, and Piggy Bank data per profile.
- Piggy Bank can be toggled off per profile.
- Import/export of all local app data.
- Automatic migration of existing `littleTransfers.v2` data into Rachel's profile.
- Check 1, Check 2, and optional Check 3 remain universal.

## v3.1 — Dark Mode
- Full dark palette based on the original Little Transfers colors.
- Deep indigo/navy backgrounds, cream text, coral/aqua/plum accents.
- Dark styling across profile selection, dashboard, goals, Piggy Bank, Spend vs Save, setup, and peek mode.
- Theme toggle in profile setup.


## v3.1.1 — Profile Navigation Polish
- Replaced the single **Profile** button in the dashboard header with two dedicated actions.
- **👀 Peek** opens the other profile directly in full read-only mode.
- **Switch** opens the profile picker and changes the active editable profile.
- Keeps the existing read-only protection so neither person can alter the other profile’s logs or setup while peeking.

## Existing v2.1 behavior retained
- Piggy Bank has a planned target of $0 and never reduces “left to transfer this month.”
- Optional “intended for” notes group across months as delayed-gratification history.
- Piggy withdrawals reduce the Piggy balance without erasing historical saving credit.
- Spend vs Save compares current-income card spending (`card paid - Piggy-funded spending`) against new GOAL contributions; BILLS are excluded.

## Install / update on GitHub Pages
Upload the contents of this folder to the repository root, replacing the old files. Be sure to replace `sw.js` so the cache updates to v3.1.1. Keep the same GitHub Pages URL to preserve browser-local data.

## Data
All data remains in browser `localStorage`. Export a backup from Setup before clearing Safari website data or moving devices.
