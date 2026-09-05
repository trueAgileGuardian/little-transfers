# Little Transfers v3.2.1

A local-first, phone-friendly PWA for tracking manual transfers, savings habits, delayed gratification, and current-income spending.

## v3.2.1 — Transfer History Edit Fix
- Restored **Edit** controls for ordinary Bill and Goal transfer-history entries that were accidentally dropped in the v3.2 combined-history refactor.
- Transfer edits can update the **amount** and **paycheck/check number**.
- Piggy Bank transfer edits can also update the optional **“intended for”** note.
- Credit-card payment edit/delete behavior remains unchanged.
- No data-model changes; existing v3.x local data carries forward.

## v3.2 — Insights & Workflow

### New Insights page
- Replaces the old **Spend vs Save** tab with a broader **Insights** page focused on the current month.
- Keeps the existing Spend vs Save scale and current-income calculation: `credit card paid - Piggy-funded spending` versus new GOAL savings.
- Adds a first-person monthly review in a speech bubble from the active profile emoji/avatar (or initial if no emoji).
- Adds up to **3 habit insights** at a time:
  - at least one positive observation,
  - no more than one neutral **“Consider…”** reminder,
  - no shaming or grading when spending is higher.
- Looks for opportunities to reinforce useful habits such as saving consistently, fully funding goals, making extra contributions, delaying gratification, planning purchases ahead, using previously saved Piggy money, and saving more than current-income spending when it happens.
- Adds a GOAL-attention pie chart showing the share of this month’s GOAL contributions by category rather than emphasizing running totals.
- Piggy Bank interpretation now calls out both money **saved ahead this month** and spending **funded from prior Piggy savings**.
- Streaks are intentionally deferred until there is more history to make them meaningful.

### Transfers workflow
- **Credit card paid?** moves from Spend vs Save onto the Transfers page.
- Placement is now: **BILLS → GOALS → CREDIT CARD PAID? → TRANSFER HISTORY**.
- Supports multiple credit-card payments in the same month.
- Every credit-card payment is associated with **Check 1, Check 2, or Check 3**.
- Credit-card payments now appear directly in Transfer History alongside transfer activity.
- Card-payment history entries can be edited or deleted.

### Goal ordering
- Added per-profile goal ordering in Setup.
- BILLS can be reordered within BILLS and GOALS within GOALS using reliable mobile-friendly **↑ / ↓** controls.
- The selected order is used on Transfers and where goal order appears elsewhere, including the Insights pie legend.

### Bottom navigation
New order:
1. **Insights**
2. **Transfers**
3. **Piggy Bank**
4. **Setup**

## v3.0 — Profiles & Custom Setup
- Multi-profile support for Rachel and Matthew.
- Profile picker with user-chosen emoji/avatar and remembered last profile.
- Full read-only 👀 peek into the other profile.
- First-time setup wizard; Matthew can start blank or copy Rachel's setup.
- Configurable Bills, Goals, and flexible/no-target goals.
- Per-paycheck, per-month, and flexible target cadences.
- Optional third-paycheck contribution behavior for per-check goals.
- Goal emoji modes: Auto, Custom, or None.
- Separate contribution, card-payment, Spend/Save, and Piggy Bank data per profile.
- Piggy Bank can be toggled off per profile.
- Import/export of all local app data.
- Automatic migration of existing `littleTransfers.v2` data into Rachel's profile.

## v3.1 — Dark Mode
- Full dark palette based on the original Little Transfers colors.
- Deep indigo/navy backgrounds, cream text, coral/aqua/plum accents.
- Theme toggle in Setup.

## v3.1.1–v3.1.2 — Profile Navigation Polish
- Replaced the ambiguous Profile control with **👀 Peek** and **Switch**.
- In read-only Peek mode, **👀 Peek** becomes **↩ Return** for a direct return to the active editable profile.

## Existing Piggy Bank behavior retained
- Piggy Bank has a planned target of $0 and never reduces “left to transfer this month.”
- Optional “intended for” notes group across months as delayed-gratification history.
- Piggy withdrawals reduce the Piggy balance without erasing historical saving credit.
- Piggy withdrawals are a funding source: they reduce the portion of card spending treated as current-income spending rather than counting as new savings again.

## Install / update on GitHub Pages
Upload the **contents** of this folder to the repository root and replace the old files. Be sure to replace `sw.js` so the cache updates to v3.2.1. Keep the same GitHub Pages URL to preserve browser-local data.

## Data
All data remains in browser `localStorage` under the existing v3 data store, so v3.1.x data carries forward. Export a backup from Setup before clearing Safari website data or moving devices.
