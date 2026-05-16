# ⚛ Black-Mozart — Interactive Lab

> Browser-based physics engines, simulations, and interactive experiments. No downloads. No installs. Just open and play.

**Live site → [Black-Mozart.github.io](https://Black-Mozart.github.io)**

---

## Projects

| # | Project | Status | Link |
|---|---------|--------|------|
| 001 | Universe Engine — N-body gravity simulator | ✅ Live | [Launch](https://Black-Mozart.github.io/universe-engine) |
| 002 | Coming soon | 🔧 WIP | — |
| 003 | Coming soon | 🔧 WIP | — |

---

## Universe Engine

A real-time gravitational physics simulator running entirely in the browser.

**Physics:**
- Barnes-Hut quadtree — O(N log N) gravity
- Velocity Verlet integration — energy-conserving orbits
- Collision merging + high-speed fragmentation
- Supernova shockwaves with radial impulse
- Black hole accretion + gravitational lensing shader

**Controls:**

| Input | Action |
|-------|--------|
| `LMB drag` | Spawn body (drag = velocity direction) |
| `LMB click` body | Lock camera to follow it |
| `RMB drag` | Pan camera |
| `RMB click` | Spawn menu at cursor |
| `Scroll` | Zoom toward cursor |
| `WASD / arrows` | Free-fly through space |
| `F` | Release follow / free camera |
| `SPACE` | Pause / unpause |
| `1` / `P` | Spawn mode: Planet |
| `2` / `S` | Spawn mode: Star |
| `3` / `H` | Spawn mode: Black Hole |
| `4` | Spawn mode: Random |
| `N` | Supernova nearest body to cursor |
| `M` | Supernova the biggest body |
| `T` | Toggle motion trails |
| `G` | Toggle glow |
| `B` | Toggle bloom shader |
| `C` | Clear all bodies |
| `R` | Reset demo solar system |

---

## Stack

- Vanilla JavaScript — zero dependencies, zero frameworks
- HTML5 Canvas 2D
- Typed arrays (`Float32Array`) for physics performance
- Software bloom via canvas compositing
- KaTeX for math rendering (Learn tab)

---

## Repo Structure

```
Black-Mozart.github.io/
├── index.html              ← Portfolio homepage
└── universe-engine/
    └── index.html          ← Universe Engine app
```

---

## Adding a New Project

1. Build your project as a single `index.html`
2. Create a new folder in this repo e.g. `my-project/`
3. Drop `index.html` inside it
4. Open the portfolio `index.html`, find the card marked `002` or `003`
5. Update the title, description, tags
6. Change `status-soon` → `status-live`
7. Set the `href` to `https://Black-Mozart.github.io/my-project`
8. Push — it's live

---

*Built with Vanilla JS · [@saphlume_](https://instagram.com/saphlume_)*
