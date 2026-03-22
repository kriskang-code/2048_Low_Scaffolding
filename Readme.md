# 🌌 2048 Galaxy

**Merge the cosmos. Reach the core.**

Ever wanted to puzzle your way through the galaxy? 2048 Galaxy is a space-themed take on the beloved 2048 puzzle game, crafted entirely with HTML, CSS, and JavaScript. Slide numbered tiles around a 4×4 grid, combine matching numbers, and chase the elusive **2048** tile. But this isn't just any puzzle game — immersive cosmic visuals, procedurally generated sound effects, and three strategic power-ups are here to help (or challenge!) you along the way.

---

## 🎮 How to Play

Ready to master the grid? Here's everything you need to know.

### Basic Controls

#### ⌨️ Keyboard

- **Move tiles** — Use arrow keys (`↑` `↓` `←` `→`) or WASD (`W` `A` `S` `D`)
- **Undo a move** — Click the **↩ Undo** button on screen
- **Swap two tiles** — Click **⇄ Swap** or press `X` to swap any two tiles
- **Remove a tile** — Click **⊗ Remove** or press `B` to clear a tile from the board
- **Start fresh** — Click **New Game** to begin again
- **Mute/unmute** — Click the **🔊** button to toggle sound on and off

#### 📱 Mobile & Tablet

- **Move tiles** — Swipe your finger in any direction
- **Undo** — Tap the **↩ Undo** button
- **Swap** — Tap the **⇄ Swap** button
- **Remove** — Tap the **⊗ Remove** button
- **New Game** — Tap **New Game**
- **Sound** — Tap the **🔊** button

### The Rules (Simple!)

1. **Slide** — Push tiles in one direction using arrow keys or swipes. All tiles slide as far as they can go.
2. **Merge** — When two tiles with the **same number** bump into each other, they fuse into one tile worth **double the value** (like `2 + 2 = 4`, `4 + 4 = 8`, etc.).
3. **Spawn** — After each move, a new tile (`2` or `4`) pops up randomly on an empty spot.
4. **Score** — Every merge adds the new tile's value to your total score.
5. **Victory** — Reach the **2048** tile and you win! 🎉
6. **Keep going** — Don't stop after 2048 — see how much higher you can push your score!

---

## ⚡ Power-Ups

Sometimes you need a little help, and we've got you covered! You have **three special abilities** at your disposal — each game gives you 2 uses of each. Use them wisely and they can mean the difference between victory and defeat.

### ↩ Undo (2 uses per game)

Made a move you regret? No problem! Revert to the board state from before your last move and watch the tiles slide back smoothly to where they were. A lifesaver when you slip up and need a second chance.

### ⇄ Swap (2 uses per game)

Need to rearrange your tiles? Swap lets you exchange any two tiles on the board. Here's how:

1. Click the **⇄ Swap** button (or press `X`) to enter swap mode.
2. Click/tap your **first tile** — it'll glow so you know it's selected.
3. Click/tap your **second tile** — both briefly glow, then they trade positions.

> **Tip:** Tap the same tile again to cancel selection, or just make a regular move to exit swap mode.

### ⊗ Remove (2 uses per game)

Sometimes you just need a tile gone. Remove destroys any single tile with a stunning crimson sparkle effect and a satisfying whoosh sound.

1. Click the **⊗ Remove** button (or press `B`) to enter remove mode.
2. Click/tap the tile you want to eliminate — it dissolves in a flash of red.

> **Note:** Remove is only available when there are more than 2 tiles on the board — we gotta leave you something to work with!

---

## 🏆 Goal

Simple yet challenging: **Reach the 2048 tile.** Merge smaller numbers together, building up from 2, 4, 8, and beyond until you finally craft that legendary 2048 tile. Once you get there, you win!

But don't stop there — keep the momentum going and see how high you can push that score. Some players love the puzzle of optimizing, while others want to dominate the leaderboard. Play your way!

---

## 💀 Game Over

The game comes to an end when:

- **The board fills up** (all 16 cells have tiles), **and**
- **No matches left** — no adjacent tiles have the same value, so no merges are possible.

When you reach this point, game over! Don't worry though — just hit **Play Again** to start a fresh run and give it another go.

---

## 💡 Tips & Tricks

Want to boost your game? Here are some strategies that work:

- **Own a corner** — Build your highest-value tile in a corner and camp there. It's your fortress.
- **Be directional** — Pick a primary direction (left, right, up, or down) and favor it. This keeps your board organized and prevents chaos.
- **Save power-ups for crunch time** — Don't burn through undo, swap, and remove early. Save them for tight situations where a single power-up saves your entire run.

---

## ✨ What Makes It Special

This isn't just another 2048 clone. Here's what sets 2048 Galaxy apart:

### 🌠 A Cosmic Universe

Dive into a fully immersive space experience. Animated star fields twinkle around you, nebulae drift lazily in the background, and a mysterious rotating black hole pulls at the center. Each tile tier gets its own unique color inspired by the cosmos — from cool blues and purples to brilliant reds and golds.

### 🔊 Sounds Made Dynamically

All sounds are created in real-time using the **Web Audio API** — no pre-recorded audio files. Every action has its own unique sonic signature: tile slides whoosh, merges chime with tier-specific tones, spawns pop, undos rewind, swaps zap, removes explode, and victory fanfares soar. The audio is part of the experience.

### 🎆 Mesmerizing Merge Effects

Watch tiles merge with space-themed shockwaves and glowing auras. The higher the tile value, the more intense the effect — higher tiles trigger particle bursts, pulsing rings, and dramatic color shifts that scream cosmic energy.

### 🔴 Smooth Remove Animations

When you remove a tile, it doesn't just disappear — it dissolves in a crimson sparkle of particles with dark ember trails and an expanding red glow ring. It's clean, it's professional, and it feels satisfying.

### 📱 Works Everywhere

Whether you're on desktop, tablet, or mobile, the game adapts perfectly. Touch swipe controls, responsive grid sizing, and optimized layouts ensure a great experience on any screen size.

### 💾 Your Best Score Saved

Your best score is automatically saved in local storage and persists across sessions, so you can come back and try to beat your personal record.

---

## 🗂 Project Structure

```
2048game/
├── index.html              # Main game page
├── style/
│   ├── main.css            # Core layout, tiles, responsive design
│   └── space-animations.css # Space effects — merges, remove, glows
├── js/
│   ├── application.js      # App entry point
│   ├── game_manager.js     # Core game logic, moves, power-ups
│   ├── grid.js             # 4×4 grid data structure
│   ├── tile.js             # Tile model
│   ├── input_manager.js    # Keyboard, touch, and button input
│   ├── html_actuator.js    # DOM rendering and animations
│   ├── sound_manager.js    # Procedural Web Audio sound effects
│   ├── space-effects.js    # Background space particle effects
│   └── storage_manager.js  # LocalStorage for best score
└── README.md
```

---

## 🚀 Getting Started

No complicated setup or dependencies — just pure, ready-to-play fun! Here's all you need to do:

1. **Clone or download** this repository to your computer.
2. **Open `index.html`** in your favorite modern browser (Chrome, Firefox, Safari, Edge, etc.).
3. **Start playing!** No installation required.

**Want to serve it locally?** If you have Node.js set up, run:

```bash
cd 2048galaxy
npx serve .
```

Then open the URL shown in your terminal (usually `http://localhost:3000`) and play!

---

## 🛠 Built With

Created with pure web technologies and zero external dependencies:

- **HTML5** — Clean, semantic markup that scales to any screen
- **CSS3** — Grid layouts, smooth animations, custom properties, and responsive design
- **Vanilla JavaScript** — No frameworks, no libraries, just pure JS doing what it does best
- **Web Audio API** — Cutting-edge procedural sound synthesis for dynamic audio generation

---

## 📜 License

This project is open source and available for personal and educational use. Fork it, modify it, learn from it — enjoy!

---

<p align="center">
  <strong>2048 Galaxy</strong> — Merge the cosmos. Reach the core. 🌌
  <br>
  <em>Play now and chase that 2048!</em>
</p>
