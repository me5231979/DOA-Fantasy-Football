# DOA Fantasy Football — Draft War Room

A single-file fantasy football draft assistant. Record every pick in your snake draft —
yours and all other teams' — and get live recommendations for your next pick built from
that data.

## Features

- **League setup**: 4–16 teams, your draft slot, PPR / Half-PPR / Standard scoring,
  fully configurable lineup (QB/RB/WR/TE/FLEX/K/DST/bench), editable team names.
- **Pick tracking**: one-click drafting assigns the player to whichever team is on the
  clock; snake order is handled automatically. Live draft board grid, per-team rosters,
  pick log with undo.
- **Recommendations**: the top five picks for your slot, ranked by value over replacement
  (position curves sized to your league and scoring), positional tier scarcity, your open
  starter/FLEX slots, and the probability each player survives until your next pick —
  each with plain-English reasons. Kickers and defenses are held back until the closing
  rounds.
- **Your data, your board**: ships with an editable 2026 preseason player pool. Import
  fresh rankings any time via CSV (a FantasyPros "Download CSV" export works as-is);
  already-drafted players are re-matched by name. Add missing players in-app.
- **Persistence**: state saves to `localStorage` automatically, with JSON export/load for
  backups or moving a draft between devices. When hosted as a Claude artifact, the draft
  also auto-saves into the artifact itself, so it follows you across devices.

## Run

Static site — no build step, no dependencies. Serve the repo root:

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

Or point GitHub Pages / Vercel at this repository and it works as-is.
