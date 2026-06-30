# Can You Free Saddam? — THE BUNKER 🔥💧

A browser-based "pull the pins" physics puzzle, inspired by the classic mobile-ad meme —
now a **15-level descent through a collapsing 5-floor bunker** with falling sand, molten lava,
water, acid, levers, gates, fans and boulders.

**No build step, no dependencies.** Just open `index.html` in a browser.

## How to play

**Read the pins before you pull. Don't just pull everything — most levels will kill him if you do.**

- 🟡 **Gold = sand** — drop it to **bury the prisoner** so the lava can't reach him.
- 🟠 **Orange = fire (lava)** — release it only **after** he's buried (it cools to rock on the sand).
- 🟢 **Green = acid** — a **trap**: it drills straight down through sand and rock to kill him. **Never pull it.**
- 🔵 **Blue = water** — **quenches lava** (→ obsidian) and is the only cure for fire you can't bury…
  but it **drowns** a prisoner who isn't covered yet.
- Some pins are **locked** (red padlock) until you pull the right one first — find the order.
- **Levers** open **sluice gates**; **fans** blow falling sand across the chamber; **boulders** drop
  straight down to bury him in rubble.

> **Order is everything**, and **more moves = less IQ**. Solve each level in par or fewer for ★★★.

> **More moves = less IQ.** Each level has a par; clear it in par or fewer for **★★★**.

## The bunker (5 floors · 15 levels)

| Floor | Theme | Levels |
|------|-------|--------|
| 1 · Cell Block | sand + lava, ordered/locked pins | Lights Out · Chain of Command · Crossfire |
| 2 · The Furnace | overhead lava, multi-source fire | Overflow · Twin Burners · Meltdown |
| 3 · Waterworks | water + quench + sluice gates | First Drop · Sluice Gates · High Tide |
| 4 · Machine Room | fans · boulders · acid trap | Conveyor · Dam It · Clockwork |
| 5 · The Core | everything, **multiple prisoners** | Two Cells · The Gauntlet · The Core |

A **bunker-map level select** lets you jump to any level; stars and best moves are saved in your browser.

## Mechanics (engine)

Custom falling-sand cellular automaton on a 220×130 grid (rendered 4× on `<canvas>`):
sand piles and caps; lava flows, cools to rock on contact, and is quenched to obsidian by water;
water seeks its level and drowns; acid dissolves terrain; boulders fall straight into dams;
levers toggle gates; fans push fluids. Web Audio sound effects (no audio files) with a mute toggle.

## Run locally

Open `index.html` directly, or serve the folder:

```sh
npx http-server -p 8123     # then visit http://localhost:8123
```

## Play online (GitHub Pages)

Enable **Settings → Pages → Deploy from branch → `main` / root**, then visit
`https://mannixadev.github.io/FreeSaDamn/`.
