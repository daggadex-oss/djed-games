# djed-games

Games built for Djed. One repo, one game per folder — see `GAME_BUILDING_PLAYBOOK.md` in `docs/` for the toolkit, checklist, and design philosophy behind all of them.

## Structure

```
games/<name>/     — each game is fully self-contained (own index.html, manifest, icons)
starters/         — reusable single-file starting points (Kaplay, Phaser tiers)
docs/             — the game-building playbook
index.html        — landing page linking to every live game
```

## Live games

- **DJed's Pixel Pals** — `games/pixel-pals/`

## Adding a new game

1. Copy the right tier from `starters/` (or start from a plain canvas, see the playbook).
2. Build it inside a new `games/<name>/` folder — no build step, no npm install.
3. Add a link to it in the root `index.html`.
4. Push to `main` — GitHub Pages redeploys automatically.

## Deployment

Served via GitHub Pages from the `main` branch, repo root. No build process — every file here is served as-is.
