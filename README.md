# ⚛ Black-Mozart — Interactive Lab

> Browser-based physics engines, simulations, and interactive experiments. No downloads. No installs. Just open and play.

**Live site → [Black-Mozart.github.io](https://Black-Mozart.github.io)**

---

## Projects

| # | Project | Status | Link |
|---|---------|--------|------|
| 001 | Universe Engine — N-body gravity simulator | ✅ Live | [Launch](https://Black-Mozart.github.io/universe-engine) |
| 002 | Gravity Field Simulator — space-time curvature mesh | ✅ Live | [Launch](https://Black-Mozart.github.io/gravity-sim) |
| 003 | Quantum Atom Simulator — 3D interactive orbitals | ✅ Live | [Launch](https://Black-Mozart.github.io/atom-sim) |

---

## 001 · Universe Engine

Real-time N-body gravitational physics simulator.

**Physics:**
- Barnes-Hut quadtree — O(N log N) gravity
- Velocity Verlet integration — energy-conserving orbits
- Collision merging + high-speed fragmentation
- Supernova shockwaves with radial impulse
- Black hole accretion + gravitational lensing bloom shader

**Controls:**

| Input | Action |
|-------|--------|
| `LMB drag` | Spawn body — drag direction = velocity |
| `LMB click` body | Lock camera to follow it |
| `RMB drag` | Pan camera |
| `RMB click` | Spawn menu at cursor |
| `Scroll` | Zoom toward cursor |
| `WASD / arrows` | Free-fly through space |
| `F` | Release follow / free camera |
| `SPACE` | Pause / unpause |
| `1` / `P` | Spawn: Planet |
| `2` / `S` | Spawn: Star |
| `3` / `H` | Spawn: Black Hole |
| `4` | Spawn: Random |
| `N` | Supernova nearest body to cursor |
| `M` | Supernova the biggest body |
| `T` | Toggle motion trails |
| `G` | Toggle glow |
| `B` | Toggle bloom shader |
| `C` | Clear all bodies |
| `R` | Reset demo solar system |

---

## 002 · Gravity Field Simulator

Einstein's rubber sheet — real-time 3D space-time curvature visualization.

**Features:**
- 3D perspective mesh that deforms toward every mass in real-time
- Depth-colored grid: flat space = blue, deep gravity well = magenta
- N-body orbital physics with Velocity Verlet integration
- Gravitational wave ripples on body interactions
- Test particle emitter — shoot particles along geodesics

**Controls:**

| Input | Action |
|-------|--------|
| `LMB drag` | Spawn body with velocity |
| `RMB drag` | Pan camera |
| `Scroll` | Zoom |
| `T` | Shoot test particle |
| `W` | Toggle gravitational waves |
| `G` | Toggle grid resolution |
| `SPACE` | Pause / unpause |
| `C` | Clear all bodies |
| `R` | Reset demo |
| `1` | Spawn: Planet |
| `2` | Spawn: Star |
| `3` | Spawn: Singularity |

---

## 003 · Quantum Atom Simulator

Interactive 3D quantum mechanical atom — drag to rotate, browse 36 elements.

**Features:**
- Full 3D perspective rendering — drag to rotate, scroll to zoom
- 36 elements: Hydrogen (Z=1) to Krypton (Z=36)
- 3 visualization modes:
  - **Bohr Model** — classical electron orbits
  - **Quantum Cloud** — probability density point cloud
  - **Orbital Shapes** — s / p / d / f orbital geometries in 3D
- Toggle individual electron shells (K, L, M, N)
- Click any electron to excite it → photon emission → spectral line appears
- Real emission wavelengths (nm) shown in spectrum bar
- Quantum numbers panel (n, l, ml, energy in eV)
- Nucleus shows protons (red) + neutrons (grey) packed in 3D

**Controls:**

| Input | Action |
|-------|--------|
| `Drag` | Rotate atom in 3D |
| `Scroll` | Zoom in / out |
| `Click electron` | Excite → emission |
| `← →` arrows | Previous / next element |
| `↑ ↓` arrows | Jump 10 elements |
| Shell buttons | Toggle shell visibility |
| Mode buttons | Switch visualization mode |

---

## Stack

- Vanilla JavaScript — zero dependencies, zero frameworks
- HTML5 Canvas 2D
- Typed arrays (`Float32Array`) for physics performance
- Manual 3D perspective projection engine
- Software bloom via canvas compositing
- KaTeX for math rendering (Universe Engine learn tab)

---

## Repo Structure

```
Black-Mozart.github.io/
├── index.html              ← Portfolio homepage
├── universe-engine/
│   └── index.html          ← Universe Engine
├── gravity-sim/
│   └── index.html          ← Gravity Field Simulator
└── atom-sim/
    └── index.html          ← Quantum Atom Simulator
```

---

## Adding a New Project

1. Build your project as a single `index.html`
2. Create a new folder in this repo e.g. `my-project/`
3. Drop `index.html` inside it
4. Open the portfolio `index.html`, find the next card slot
5. Update title, description, tags, status and href
6. Push — it's live in ~2 minutes

---

*Built with Vanilla JS · [@saphlume_](https://instagram.com/saphlume_)*
