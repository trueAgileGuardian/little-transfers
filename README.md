# Little Transfers v2.1

A phone-first local PWA for tracking manual transfers, mandatory bills, savings goals, credit-card payments, and delayed-gratification Piggy Bank savings.

## v2.1 highlights
- Piggy Bank has a planned target of $0, so its contributions never reduce “left to transfer this month” or advance the planned-transfer progress bar.
- Optional “intended for” labels on Piggy Bank contributions group across months while the money remains one flexible balance.
- Piggy Bank spending/withdrawals reduce the available Piggy balance without erasing historical savings credit.
- Spend vs Save treats Piggy withdrawals as a funding source: card paid minus Piggy-funded spending = current-income spending, compared against new GOAL contributions.
- BILLS remain excluded from the Spend vs Save comparison.

## GitHub Pages update
Upload/replace all files in the repository root and commit. The service worker cache version is bumped for v2.1. Existing `littleTransfers.v2` local data is preserved and extended in-place.

## Data
All financial activity remains in browser localStorage on the device. Clearing Safari website data can erase it.
