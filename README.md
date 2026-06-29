# Can You Free Saddam? 🔥

A browser-based "pull the pins" physics puzzle, inspired by the classic mobile-ad meme.
Molten lava, falling sand, and a buried prisoner — pull the pins in the right order to keep him safe.

**No build step, no dependencies.** Just open `index.html` in a browser.

## How to play

1. Press **PLAY**.
2. Pull the **gold sand pins** to drop the sand and **bury Saddam**.
3. Then pull **every lava pin** so the lava pours onto the sand and **cools to rock**.
4. **Order is everything** — pull a lava pin too early, or before he's covered, and the molten lava burns him. Game over.

> **More moves = less IQ.** Solve each level in as few pulls as you can.

## Levels

| # | Name | Twist |
|---|------|-------|
| 1 | First Cut | Bury, then release one side lava |
| 2 | Crossfire | Lava on **both** sides |
| 3 | Triple Lock | Three sand pins to open the tank |
| 4 | Overhead | Lava hangs **directly above** Saddam — bury the centre before you drop it |

## Features

- Custom falling-sand / lava **cellular-automata physics** (sand piles, lava flows and cools)
- Hand-drawn cartoon art rendered on `<canvas>` — textured dirt cross-section, brick entrance, the grumpy air-vent monster, a spinning fan, and the "6ft" depth marker
- **Web Audio** sound effects (pin pop, sand pour, lava sizzle, win/lose stings) with a mute toggle — no audio files
- Multiple levels with a win/lose flow and a tongue-in-cheek **IQ score**

## Tech

Single self-contained HTML file — vanilla JavaScript, Canvas 2D, and the Web Audio API. ~160×90 simulation grid rendered at 6× scale.

## Run locally

Open `index.html` directly, or serve the folder:

```sh
npx http-server -p 8123
# then visit http://localhost:8123
```

## Play online (GitHub Pages)

Enable **Settings → Pages → Deploy from branch → `main` / root**, then visit:
`https://mannixadev.github.io/FreeSaDamn/`
