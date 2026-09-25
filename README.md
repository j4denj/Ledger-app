# Ledger

A tab-based cost and attendance tracker for recurring activities — think badminton lessons, tutoring, or any hobby where you want to know what it's actually costing you.

**Try it live:** https://claude.ai/artifact/TYzVVgG6txXAjfSMNsCUXe
*(Data saves automatically in the live version above — see note below if running the code elsewhere.)*

## What it does

- Create a "tab" for each activity (Badminton, Tutoring, etc.), each with its own color
- Log entries on a calendar — cost, number of people, notes
- See totals: this month, all-time, per activity, or combined across everything with the "All Activities" view
- Select multiple specific days to get a custom subtotal
- Averages per session and per person, calculated automatically
- Rename or delete activities anytime
- Light/dark mode and a few color palette options, in Settings

## Tech

Single self-contained HTML file — no build step, no dependencies, no framework. Vanilla JS.

## ⚠️ Storage note

This app uses a storage API that only works when opened through the live claude.ai link above. If you clone this repo and open `ledger.html` directly in a browser (or host it elsewhere, e.g. GitHub Pages), the interface will load correctly but data won't save — you'll see a "Storage is not available" message instead.

To actually use it with persistent data, open it via the live link. Contributions/forks that swap in a different backend (Firebase, Supabase, etc.) are welcome.

## Feedback

Feedback and bug reports welcome — open an issue here, or use the "Send feedback" link inside the app's Settings.
