# 🏏 Cric Gyan

> **An interactive, visual, and playable guide to the art and physics of cricket.**  
> Zero external frameworks. Pure Vanilla JavaScript & HTML5 Canvas.

🌐 **Live Demo:** [https://cric-gyan.vercel.app/](https://cric-gyan.vercel.app/)

---

## 🌟 Overview

**Cric Gyan** is a lightweight web application that combines a mini-arcade cricket chase game with interactive 3D/2D visual guides covering bowling trajectories, batting strokes, and stadium fielding tactics.

---

## 🚀 Modules & Features

### 1. 🎮 Playground — Last Over Chase (`index.html`)
- **The Scenario:** Need 16 runs off 6 balls with 2 wickets in hand.
- **Dynamic Physics & Deliveries:** Face real bowling variations:
  - *Pace, Yorker, Slower Ball, Off-Cutter, Bouncer, Inswinger*
- **3D Bat Swing Engine:** Custom elevation, azimuth, roll, and blade projection rendered on Canvas.
- **Timing Mechanics:**
  - ⏱ **Early Timing:** Pulls/glances towards the leg side.
  - ⏱ **Late Timing:** Steers/cuts towards the off side.
  - ⏱ **Perfect Timing:** Dispatches the ball into the night sky for **SIX!**
- **Procedural Sound:** Built with the **Web Audio API** (bat thocks, crowd cheers, timber shatter sound) — no audio files required.
- **Score Persistence:** Saves your high score in `localStorage`.

---

### 2. 🎯 Bowlers Explained (`bowling-guide.html`)
- **Dual Perspective:** Simultaneous **Top View** and **Side View** pitch trajectories.
- **Ball Physics & Variations:**
  - *Outswinger, Inswinger, Off-cutter, Leg-cutter, Off-spin, Leg-spin, Googly, Yorker, Bouncer, Slower ball*.
- **Visual Aids:** Ghost paths showing what the batter anticipates vs. the actual ball movement off the pitch.
- **Controls:** Slow-motion, Pause, Replay, and keyboard arrow navigation (`←` / `→`).

---

### 3. 🏏 Batting Explained (`batting-guide.html`)
- **Holographic 3D View:** Top-down view of 11 classic cricket strokes:
  - *Straight Drive, Cover Drive, On Drive, Square Cut, Late Cut, Pull, Hook, Sweep, Reverse Sweep, Leg Glance, Scoop (Dilscoop)*.
- **Swing Arcs & Trajectories:** Visualizes bat path, contact point, loft elevation, and shot landing zones.
- **Interactive Pitch:** Drag to rotate the pitch yaw in real time or enable auto-rotate.

---

### 4. 🏟️ Stadium Explained (`stadium-guide.html`)
- **Fielding Map:** Visual breakdown of all key fielding positions:
  - *Wicketkeeper, Slips, Gully, Silly Point, Point, Cover, Extra Cover, Mid-off, Mid-on, Mid-wicket, Square Leg, Short Leg, Fine Leg, Third Man, Long-off, Long-on, Deep Mid-wicket*.
- **Ground Markings:** Detailed explanations of the 22-yard pitch, 30-yard fielding circle, boundary ropes, off/leg side splits, and sightscreens.
- **Interactive Hologram:** Full 3D rotation, yard distance indicators, and tactical fielding insights.

---

## 🛠️ Tech Stack

- **Frontend:** HTML5, CSS3, Vanilla JavaScript (ES6+)
- **Graphics:** HTML5 2D Canvas (Custom 3D-to-2D projection math)
- **Audio:** Web Audio API (Synthesized Oscillators & White Noise)
- **Typography:** Google Fonts (*Alfa Slab One, Barlow Condensed, Orbitron, Rajdhani*)
- **Deployment:** Vercel (`cleanUrls: true`)

---

## 📂 Project Structure

```text
cricket-playground/
├── index.html           # Last Over chase game (Playground)
├── batting-guide.html   # Interactive batting stroke guide
├── bowling-guide.html   # Bowling trajectory & delivery guide
├── stadium-guide.html   # Stadium & fielding positions hologram
├── vercel.json          # Vercel deployment configuration
└── README.md            # Project documentation
```

---

## ⚡ Getting Started Locally

No build steps, bundlers, or `npm install` needed!

1. **Clone the repository:**
   ```bash
   git clone https://github.com/<YOUR_USERNAME>/<REPO_NAME>.git
   cd <REPO_NAME>
   ```

2. **Run locally:**
   - Open `index.html` directly in any modern web browser.
   - Or use a local development server (e.g. VS Code Live Server or Python):
     ```bash
     # Python 3
     python -m http.server 8000
     ```
   - Open `http://localhost:8000` in your browser.

---

## 🕹️ Controls

| Screen | Action | Key / Input |
|---|---|---|
| **Playground** | Swing bat / Take guard | `Space` / `Enter` / Screen Tap |
| **Playground** | Toggle Sound | Sound button (`🔊` / `🔇`) |
| **Guides** | Next / Previous Technique | `Arrow Right` (`→`) / `Arrow Left` (`←`) |
| **Guides (3D)** | Rotate pitch view | Pointer Drag (Touch / Mouse) |
| **Guides** | Playback Controls | Replay, Slow-mo, Pause buttons |

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

