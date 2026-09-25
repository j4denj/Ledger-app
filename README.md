# Ledger

A tab-based cost and attendance tracker for recurring activities — think badminton lessons, tutoring, or any hobby where you want to know what it's actually costing you and your group.

**Try it live:** https://claude.ai/artifact/TYzVVgG6txXAjfSMNsCUXe
*(Data saves automatically in the live version above — see note below if running the code elsewhere.)*

## What it does

**Activities & calendar**
- Create a "tab" for each activity (Badminton, Tutoring, etc.), each with its own color and a monogram badge
- Log entries on a calendar — cost, number of people, notes
- Log an entry for *any* activity from any day, without switching tabs, via a dropdown in the entry form
- Edit or delete existing entries any time
- "Repeat last" button pre-fills an entry with your most recent session's numbers, so recurring lessons don't need retyping
- Live "$X per person" preview while typing cost and headcount

**Totals & insight**
- Totals by month, all-time, or combined across every activity via the "All Activities" view
- See which other activities also happened on a given day (badge indicators on the calendar), with a full cross-activity breakdown when you open that day
- Average cost per session and per person, calculated automatically
- Select multiple specific days to get a custom subtotal
- "Share summary" — generates a copyable text breakdown of a month's entries (per session, with per-person split) for pasting into a group chat to split costs

**Management & appearance**
- Rename or delete activities anytime (with a confirm-to-delete safety step)
- Light / dark / auto theme, plus a few curated color palettes, in Settings
- In-app feedback link

## Tech

Single self-contained HTML file — no build step, no framework, no dependencies. Vanilla JS.

## ⚠️ Storage note

This app uses a storage API that only works when opened through the live claude.ai link above. If you clone this repo and open `ledger.html` directly in a browser (or host it elsewhere, e.g. GitHub Pages), the interface will load correctly but data won't save — you'll see a "Storage is not available" message instead.

To actually use it with persistent data, open it via the live link. Contributions/forks that swap in a different backend (Firebase, Supabase, etc.) to make it fully standalone are welcome.

## Feedback

Feedback and bug reports welcome — open an issue here, or use the "Send feedback" link inside the app's Settings.

## Roadmap ideas (not yet built)

- Monthly budget/goal per activity with progress tracking
- Spend-over-time chart
- CSV export
