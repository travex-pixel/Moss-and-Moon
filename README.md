# Moss & Moon 🌙

A tiny watercolor garden you wake with a tap. One glowing seed, a chain of blooms, three sparks per round, and some very small, very round creatures.

**Play it:** open `index.html` in any modern browser. On a phone, the easiest way is GitHub Pages (see below).

## How to play

- Tap the glowing seed. It blooms and sends a ring of light out; seeds inside the ring wake and bloom in a chain.
- **Catch the wave.** The ring keeps travelling past the seeds it wakes. Any sleeping seed it touches *shimmers*; tap it while it shimmers to pull it into the live chain, for free. Tap just as the closing ring lands on it for a **Perfect** (double points and a bigger wave).
- Tapping a seed before the light reaches it does nothing except make it grumpy for a moment (it can't be caught briefly), so mashing doesn't help.
- You get **3 sparks** per round. A spark starts a new chain; catching never costs one.
- **Scoring:** the n‑th bloom of a chain is worth n moon‑drops, uncapped, so one long chain beats several short ones. Moonflowers +25, lantern mushrooms +5, bluebells +3, golden seeds double. Wake every seed for a **+40 full bloom**, plus **+30 per unused spark**.
- Combo words pop at 5, 10, 15, 20, 30 and 40: Lovely, Magical, Dreamy, Enchanting, Moonstruck, Legendary.
- Special flowers light up a big catch zone: moonflowers and lanterns send their ring much further, and a bluebell rings a second time to make a wide area catchable.
- **Today's garden** (Daily) gives everyone the same layout for the day, with its own best score.

The first garden is hand‑built to teach catching: the first time a seed shimmers, time slows right down and a hint appears.

## Music

Every garden has its own short original tune (Moonlit Lullaby, Firefly Waltz, Mossy Steps, Petal Rain, Sleepy Pond, Star Garden). Each bloom in a chain plays the next note, long chains loop it with harmony and bass, and a full bloom finishes the phrase and resolves on a chord. The tune's name is on the results card.

## Creatures and the sticker album

- **Mochi Mossling** sleeps beside the first seed, wakes on your first tap and hops at every 5th bloom.
- **Pip** peeks out from behind moonflowers.
- **Moon Moth** wakes at 500 lifetime moon‑drops and follows your blooms.
- **Nib**, a tiny moon snail, lives by the pond. Tap its shell, or catch a seed, and it peeks out.

The **sticker album** (Album button on the results card) holds 12 creature poses, each earned by a small feat: chains of 10, 25 and 35, moonflowers, 5 Perfects in one garden, catching 6 seeds in one garden, full blooms, and full blooms with a single spark. Locked stickers show as silhouettes with their goal.

Garden unlocks: golden seeds (15‑chain), cottage lights (1500 drops), moonlit meadow (4000 drops).

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
