# 🦣 Mammoth Hunt

A tiny web strategy game on a 10×10 grid. Place hunters, then watch a herd of
animals cross the map — terrain, timing, and weapon choice decide the kill.

## How to play

- **Place hunters** on walkable land before the wave. Each carries one weapon:
  - 🪨 **Rock** — cheap, low damage, decent odds on big animals.
  - 🔱 **Spear** — high damage, best against large prey.
  - 🕸️ **Net** — snares small prey outright; tangles/slows big ones.
- **Terrain** changes how fast animals move through a cell (and where hunters can stand):
  Grassland (normal), Forest & Marsh (slow — good ambush spots), Water (very slow, no standing), Rock (impassable).
- Hunters only strike animals that pass **adjacent or over** them.
- **Prey** flee straight across. **Predators** (🐺 🐻) can overrun and kill a hunter.
- Reach **1000 lbs of meat** to win. Each wave adds new terrain and reinforcements.

## Run locally

Just open `index.html` in a browser — it's a single self-contained file.

## Deploy (Fly.io)

```sh
fly deploy
```

Served as a static site via nginx (see `Dockerfile` / `fly.toml`).
