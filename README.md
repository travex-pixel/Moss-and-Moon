# Moss & Moon 🌙

A tiny watercolor garden you wake with a tap. One glowing seed, a chain of blooms, three sparks per round, and some very small, very round creatures.

**Play it:** open `index.html` in any modern browser. On a phone, the easiest way is GitHub Pages (see below).

## How to play

- Tap the glowing seed. It blooms and sends a ring of light out; seeds inside the ring wake and bloom in a chain.
- **Catch the wave.** The ring keeps travelling past the seeds it wakes. Any sleeping seed it touches *shimmers*; tap it while it shimmers to pull it into the live chain, for free. Tap just as the closing ring lands on it for a **Perfect** (double points and a bigger wave).
- Tapping a seed before the light reaches it does nothing except make it grumpy for a moment, so mashing doesn't help.
- You get **3 sparks** per level. A spark starts a new chain; catching never costs one.
- **Scoring:** the n‑th bloom of a chain is worth n moon‑drops, uncapped. Moonflowers +25, lanterns +5, bluebells +3, golden seeds double, brambles cleared +10. Wake every seed for **+40 full bloom**, plus **+30 per unused spark**.

## Levels

- A garden path of levels with **1–3 stars** each. The top bar shows your score filling toward the three stars; the first star passes the level.
- Missing the pass target just means an instant, free retry. No lives, no timers.
- Difficulty rises gently: more seeds and islands, a slightly shorter catch window, and one new idea at a time — moonflowers (level 2), lanterns (4), bluebells (7), **sleepy seeds** with nightcaps that need two lights or two taps (11), and **brambles** that block light until a flower blooms beside them (16).
- Every 5th level is a breather; every 10th is a bigger **Moon Night** with two moonflowers.
- Levels 2–100 were tuned by simulating four kinds of player (never catches, casual catcher, fast catcher, perfect timing) on several candidate gardens per level. Early levels and breathers can be passed without catching; two stars is about what a casual catcher gets; three stars needs Perfect timing but is always reachable. Beyond 100, the meadow cycles through tuned levels 61–100.
- The **map** button (top right) opens the garden path. Replay any level for more stars, or play **Today's garden**, the same layout for everyone that day.

## Help for new and returning players

- A soft paw points at exactly what to tap: straight away on the first five levels and on the first level of every visit, and later only if you pause for a while.
- The first time a seed shimmers, time slows and a hint explains catching.
- Each level opens with its goal ("Get 135 moon-drops to pass"), a one-line tip when something new appears, and a reminder of the two rules on early levels.
- Coming back after a day or more shows "Welcome back!" with the rules and the paw again.
- "One seed left!" and "So close — 1 seed from a full bloom" moments make near-misses clear.
- On Android, light vibrations accompany taps, catches, stars and full blooms. Muting sound also turns vibration off.

## Music

Every garden has its own short original tune (Moonlit Lullaby, Firefly Waltz, Mossy Steps, Petal Rain, Sleepy Pond, Star Garden). Each bloom in a chain plays the next note, long chains loop it with harmony and bass, and a full bloom finishes the phrase and resolves on a chord. The tune's name is on the results card.

## Friends (pet companions)

From level 3 a friend sits in the round button at the bottom right. Catches, Perfects, combo words and moonflowers fill the ring around it; when it's full the button bounces — tap it to use the friend's power. Tap it while it's still filling to open the **Friends** picker.

| Friend | Power | How you meet them |
|---|---|---|
| Mochi | Spark roll: one extra spark | From the start |
| Pip | Lucky peek: hops to the best seed and makes it golden (double points) | Open a moonflower |
| Moon Moth | Moonglow: slows time for a few seconds | 500 lifetime moon-drops |
| Nib | Shell shield: catches the next 3 seeds you'd miss | Catch a seed on the wave |
| Sprig | Moon-breath: flies across the garden, waking every seed in its beam (free, no spark) | Hatch the egg |

If you run out of sparks while Mochi or Sprig is ready, the round waits a few seconds for you to use them. If a level beats you twice, your friend starts the next try fully charged.

## The dragon egg

At level 8 a speckled egg appears on the hill below the cottage. Catches, Perfects, stars and full blooms warm it (tap it to see how warm). When it's warm enough it hatches at the start of your next level into **Sprig**, a baby moss dragon, who becomes your friend. Sprig grows with the stars you earn: Hatchling → Fledgling (12 stars) → Moon Dragon (36 stars), with bigger wings, longer horns and a wider beam each time.

## Creatures and the sticker album

- **Mochi Mossling** sleeps beside the first seed, wakes on your first tap and hops at every 5th bloom.
- **Pip** peeks out from behind moonflowers.
- **Moon Moth** follows your blooms once awake.
- **Nib**, a tiny moon snail, lives by the pond and peeks out when you catch seeds or tap its shell.
- **Sprig** lives on the hill once hatched.

The **sticker album** holds 15 creature poses, each earned by a small feat (long chains, moonflowers, Perfects, full blooms, hatching and growing Sprig). Locked stickers show as silhouettes with their goal.

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
