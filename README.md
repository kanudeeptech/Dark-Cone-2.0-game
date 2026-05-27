# DARK CONE 2.0 🔦

A 2D top-down horror-survival maze game built using the **Phaser 3** engine. Navigate dark corridors, manage your flashlight's battery, avoid a hunting monster, and collect keys to make your escape!

---

## 🎮 Gameplay & Rules

* **Objectives**: 
  1. Find **2 hidden keys** (🔑) randomly placed in the maze.
  2. Locate the **escape door** (🚪) which remains hidden in the shadows until both keys are collected.
  3. Enter the door to escape and survive!
* **Controls**:
  * **Movement**: Use `W` `A` `S` `D` or the **Arrow Keys**.
  * **Flashlight**: Hold **Left-Click** (or **Tap & Hold** on mobile) to project a 2D raycasted light beam in the direction of your mouse cursor.
* **The Flashlight & Battery (⚡)**:
  * Your flashlight is your only way to see keys and the monster.
  * Shining the light **drains the battery**.
  * Releasing click turns off the flashlight, allowing the battery to **recharge** over time.
  * When battery drops below `15%`, your flashlight will begin to flicker erratically.
* **The Monster (👾)**:
  * A monster wanders the maze, tracking your path.
  * **Freezing mechanic**: The monster will **freeze in place** as long as you shine your flashlight directly on it.
  * If the monster catches you, the game ends.

---

## ⚡ Key Features

* **Advanced 2D Raycasting**: Dynamic visibility polygon calculations simulate realistic light and shadows around maze corners.
* **Ambient Sound System**: Custom background horror track, looping monster proximity sounds (crunching) that trigger when the beast is near, and responsive win/lose cues.
* **Lively Main Menu**: Dynamic searchlight beam sweep, ambient floating fog particles, and formatted instruction card.
* **End Game Celebrations**: Color-shifting confetti particle emitters and an escape timer overlay.
* **Randomized Gameplay**: Spatially constrained randomized key placement ensures keys spawn far apart and never overlap, offering a fresh experience every round.

---

## 🚀 Installation & Local Setup

Because the game loads custom audio assets (WAV/MP3 files), browser security rules (CORS policies) prevent it from loading directly off your local disk via the `file://` protocol. **You must run the game using a local HTTP server.**

### Step 1: Clone the repository
```bash
git clone https://github.com/your-username/Dark-Cone-2.0-game.git
cd Dark-Cone-2.0-game
```

### Step 2: Start a local server
Choose one of the quick options below based on your system setup:

#### Option A: Node.js (Recommended)
If you have Node.js installed, run:
```bash
# Starts a server instantly without manual installation
npx -y http-server -p 8080
```

#### Option B: Python
If Python is installed on your machine, run:
```bash
python3 -m http.server 8080
```

### Step 3: Play the game
Open your browser and navigate to:
👉 **[http://localhost:8080](http://localhost:8080)**

*(Note: If you run into outdated graphics or layout bugs, perform a **Hard Refresh** via `Cmd + Shift + R` on Mac or `Ctrl + F5` on Windows to clear your browser's cache.)*
