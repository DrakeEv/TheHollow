# The Hollow

A moody, first-person 3D exploration experience built entirely in a single HTML
file with [Three.js](https://threejs.org/). You wake at the edge of a
bioluminescent forest and explore on foot, searching for eight glowing memory
orbs scattered through the trees — each one reveals a fragment of an unsettling
short narrative. Built as an experiment to see what Three.js could do for
atmospheric, game-like web experiences.

## Key Features

- **First-person exploration** — WASD movement with pointer-lock mouse look
- **Procedurally generated forest** — 150 trees placed with a seeded RNG, so the
  world is the same every time
- **Bloom post-processing** — glowing canopies, orbs, and drifting light motes
  via `UnrealBloomPass`
- **Collectible narrative fragments** — 8 hidden orbs, each revealing a short
  piece of lore when found, tracked in an on-screen HUD
- **Pause/resume flow** — pointer-lock unlock triggers a pause overlay

## Tech Stack

- [Three.js](https://threejs.org/) (r160) — WebGL scene, lighting, and
  post-processing, loaded via CDN import map
- Vanilla HTML, CSS, and JavaScript (ES modules) — no build step, no
  dependencies to install

## Running Locally

This is a single static HTML file, but browsers block ES module imports over
`file://`, so serve it locally instead:

```bash
# from the repo directory
npx serve .
# or: python -m http.server
```

Then open the printed local URL, click to enter, and use **WASD** to move,
**mouse** to look, and **Esc** to pause.

## Live Demo

**https://drakeev.github.io/TheHollow/**

## License

MIT — see [LICENSE](LICENSE).
