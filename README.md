# Golazo · World Cup 2026 Lineup Generator

Live, editable football lineups for the 2026 FIFA World Cup, powered by the ESPN API.
A single self-contained HTML file — no build step, no dependencies.

## Features

- **Real data, real formations** — pulls live rosters, formations, and player positions straight from ESPN
- **Live score & clock** — auto-refreshes every 30s while a match is in play
- **Both-teams view** — see both lineups facing off on one pitch
- **Drag & drop** — reposition any player; edit name, number, and position
- **Real player jerseys** and team flags/crests
- **Goal / card / substitution markers** on the pitch
- **Click a player** for their match stats
- **Export** to PNG or plain-text lineup
- **Persistence** — your edits are saved per match in localStorage
- **Golazo watermark** baked into every lineup
- Fully mobile responsive

## Run it

Because the app fetches from the ESPN API and loads a local logo, serve the folder
over HTTP (opening the file directly with `file://` will not work):

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000/wc2026-lineup-editor.html>.

## Files

- `wc2026-lineup-editor.html` — the entire app
- `golazo-logo.png` — watermark logo
