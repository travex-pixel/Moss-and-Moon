# Moss & Moon 🌙

A tiny watercolor garden you wake with a tap. One glowing seed, a chain of blooms, three sparks per round, and some very small, very round creatures.

**Play it:** open `index.html` in any modern browser. On a phone, the easiest way is GitHub Pages (see below).

## How to play

- Tap the glowing seed. It blooms and sends a pulse of light into nearby seeds, which bloom in a chain.
- You get **3 sparks** per round. A spark is spent only when you tap a sleeping seed. Tapping flowers or grass is free (and fun).
- **Scoring:** the n‑th bloom of a chain is worth n moon‑drops (capped at 10). Moonflowers add +25, lantern mushrooms +5, bluebells +3, a golden seed doubles. Wake every seed for a **+40 full bloom** bonus.
- Choose where to spend sparks: a chain that reaches a moonflower pulls in a wide circle of seeds.
- **Today's garden** gives everyone the same layout for the day, with its own best score.

## Creatures

- **Mochi Mossling** — sleeps beside the first seed, wakes on your first tap, hops on long chains.
- **Pip** — shy and long‑eared, peeks out from behind moonflowers.
- **Moon Moth** — unlocks at 300 lifetime moon‑drops and follows your blooms.

More unlocks: golden seeds (12‑chain), cottage lights (800 drops), moonlit meadow (2000 drops).

## Put it on your phone (GitHub Pages)

1. In this repository: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
2. Open `https://travex-pixel.github.io/Moss-and-Moon/` on your phone.
3. Optional: in Chrome on Android, use **Add to Home screen** — the manifest and icon make it launch full‑screen.

Links shared from that URL show the preview image (`og.png`) on messaging apps and social sites.

## Tech

- Single `index.html`: plain HTML, CSS and JavaScript. No build step, no dependencies, no network calls, works offline once loaded.
- Canvas 2D for the scenery, particles, flowers and creatures (all procedural). HTML for the few UI pieces.
- Web Audio API for original procedural sound (pentatonic chimes; a long chain plays a rising melody). Mute is persisted.
- `localStorage` for best score, best chain, unlocks and today's best; the game runs fine when storage is blocked.
- Respects `prefers-reduced-motion`, keyboard playable (arrows + Enter, M mute, R new garden), 44px+ touch targets.

Everything (art, creatures, sound) is original to this project.
