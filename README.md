# Dapur Kilat — Warung Nusantara

A complete, original cooking game for the Make.Fun bounty "Make the best cooking game".
It runs offline in a desktop browser from its own static files — no network requests.

## How to play
- 3 customers order at once on the order board, each with a recipe (3–5 ingredients) and its own timer.
- Click an order, click ingredients on the counter, click Cook (~2s), then Serve to the right customer before their timer runs out.
- Recipes: Nasi Goreng, Mie Goreng, Sate Ayam, Soto Ayam.
- Score/coins (target 150), combo multiplier up to x6, 3 stars, 120-second shift, start / pause / game over / win screens.

## Controls
- Mouse: click everything (orders, ingredients, Cook, Serve, buttons).
- Keyboard: 1–6 pick an ingredient, Space/Enter serve, P pause, R restart.

## Run it
- Play: open `game/index.html` in desktop Chrome, or run `node serve.ts` and open http://localhost:8080
- Build the hand-in: `mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts` — copies game/ and screenshots/ to out/ and writes out/dossier.json with buildDossier from vendor/makefun-game.ts (starter's main.ts, unchanged).

## Layout
- `main.ts` — starter's hand-in program (unchanged)
- `serve.ts` — starter's tiny static server
- `vendor/makefun-game.ts` — copied unchanged from the official kit
- `game/index.html` — the whole game (single file, CSS/emoji art, WebAudio sounds, no external files)
- `screenshots/` — 4 real renders of the game running in a browser
- `shots.json` — screenshot list
- `LICENSE` — MIT (starter's)
