# Arcade

Static games hub (same idea as dicestack88.github.io). No build step, no server code,
so it can be hosted free on GitHub Pages.

## Add a game
1. Put the game's files in `games/<id>/` with an `index.html` entry point.
2. Add a line to `games.json`:
   `{ "id": "<id>", "title": "Name", "tags": ["x"], "thumb": "games/<id>/thumb.png" }`
   (`thumb` is optional. Use `"url": "https://..."` instead of a local folder to embed an external page.)

## Run locally
`python3 -m http.server 8000` then open http://localhost:8000

## Host
Push to a GitHub repo, then Settings -> Pages -> deploy from `main` / root.
