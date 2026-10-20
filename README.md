# FPS Playground — 3D Browser FPS

A fast-paced, standalone 3D First-Person Shooter web game built with **Three.js** and procedural Web Audio. Zero external build steps, runs directly in any modern browser!

🎮 **Live Demo:** [https://ani-github-24.github.io/sturdy-barnacle/](https://ani-github-24.github.io/sturdy-barnacle/)

---

## 🌟 Features

- **Standalone 3D Engine**: Built directly using Three.js (r128) via CDN with procedural sky, terrain, shadows, and lighting.
- **Synthesized Audio System**: Fully procedural sound effects (gunshots, reload, footsteps, hit markers, alerts) powered by the Web Audio API — no external audio files required.
- **Mission & Objective System**:
  - Narrative intro briefing with typewriter animation.
  - Phase 1: Clear hostile patrol units from the Ruined Outpost.
  - Phase 2: Infiltrate and secure the Enemy Base perimeter.
  - Post-game stats tracking (kills & clear time).
- **Tactical HUD**:
  - Live minimap with radar blips for enemy locations and player orientation.
  - 360° dynamic compass with compass points and directional heading.
  - Zone identification HUD (Camp, Ruined Outpost, Enemy Base).
  - Health bar, ammo counter, reload indicator, and crosshair with hit reaction.
- **Enemy AI**:
  - Multi-state behaviors: Patrol, Alert/Investigate, Chase, Attack, and Search.
  - Line-of-sight checks with raycasting, recoil, muzzle flash, and hit feedback.

---

## 🕹️ Controls

| Key / Action | Function |
| :--- | :--- |
| **W, A, S, D** | Move Forward / Left / Backward / Right |
| **Mouse** | Aim / Look (Pointer Lock) |
| **Left Click** | Fire Weapon |
| **R** | Reload |
| **Space** | Jump |
| **Shift** | Sprint |
| **Tab / Esc** | Pause / Options Menu |

---

## 🚀 GitHub Pages Setup

This repository is preconfigured for automatic GitHub Pages hosting.

### Method 1: GitHub Actions (Recommended)
1. Go to your repository on GitHub: `https://github.com/Ani-github-24/sturdy-barnacle`
2. Navigate to **Settings** > **Pages**.
3. Under **Build and deployment** > **Source**, select **GitHub Actions**.
4. The included workflow (`.github/workflows/deploy.yml`) will automatically build and deploy whenever you push to `main`.

### Method 2: Deploy from a branch
1. Go to **Settings** > **Pages**.
2. Under **Build and deployment** > **Source**, select **Deploy from a branch**.
3. Under **Branch**, select `main` and folder `/ (root)`.
4. Click **Save**.

Your site will be live at:
**https://ani-github-24.github.io/sturdy-barnacle/**

---

## 🛠️ Local Development

Simply open `index.html` in your browser or run a lightweight local static server:

```bash
# Python
python -m http.server 8000

# Node.js
npx serve .
```

Visit `http://localhost:8000` to play locally.
