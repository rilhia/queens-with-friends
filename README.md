# Queens With Friends ♛
> **Play, challenge, and learn with friends.**

**Queens With Friends** is an open-source logic puzzle engine. It was built as a response to the "leaderboard culture" of the puzzle on LinkedIn, where faked solve times and scripts often overshadow genuine skill. 

This platform returns the game to its roots: a private, honest, and transparent environment for true logic enthusiasts to sharpen their minds and challenge their peers.

---

## 🛡️ The Mission
The inspiration for this project came from observing the competitive "Queens" puzzles on LinkedIn. I noticed that instead of fostering a community of learners, the focus often shifted to displaying impossible solve times.

**Queens With Friends** solves this by:
1. **Eliminating the Central Leaderboard:** Competition happens between friends via direct challenge links.
2. **Exposing the Logic:** A built-in "Solver" which takes you through how to solve boards.
3. **Encouraging Creation:** Allowing users to architect their own challenges and validate them mathematically. 

---

## 🎮 The Rules
The goal is to place exactly **N** queens on an **N x N** grid. To reach a valid solution, you must satisfy four constraints:
1. **Row:** Exactly one queen per row.
2. **Column:** Exactly one queen per column.
3. **Region:** Exactly one queen per color-coded region.
4. **Adjacency:** No two queens can touch, even diagonally.

---

## 🚀 Key Features

### 1. The Play Tab 
* **Precision Timing:** A 3-2-1 countdown starts after you have pressed the "Start" button.
* **Controls:** Touch cells to set them to blocked or unblock them. Queens are set with a double tap. There is a "Back" button to undo a move and a "Reset" button if you want to start again.
* **State Integrity:** A full undo-stack and real-time conflict detection.

### 2. The Build Tab 
* **Greedy Snakes Algorithm:** A custom procedural generator that grows organic, connected color regions from high-dispersion seeds. Note: For smaller boards this performs quicker. Larger boards at higher complexity levels can take a while to generate.
* **Manual Design:** A "paint" tool to architect your own puzzles or modify generated puzzles. Maybe recreate a model you have seen elsewhere.
* **Logic Validator:** An internal solve-engine that audits your custom designs for connectivity and solution uniqueness before you share them.

### 3. The Solve Tab 
* **Heuristic Deduction:** Uses human-like strategies (Super-Intersections, Mutual Exclusion, and Contradiction Chaining).
* **Reasoning Log:** A step-by-step log of how the puzzle is solved with graphics on the board to guide you as well.

### 4. Zero-Server Sharing (P2P)
* No databases, no accounts, no tracking. 
* **Queens With Friends** uses **Base64 URL Encoding** to store the entire board state within the link. Simply click "Share," send the URL to a friend, and they are playing your specific board instantly.

---

## 🛠️ Technical Implementation
* **Architecture:** Single-file JS/HTML/CSS (Zero dependencies). 
* **Graphics:** Dynamic CSS for rendering across mobile and desktop.

---

## 📖 How to Use

1. **To Play:** Open the game and click "Start." Single tap to block a cell (•), double tap to place a queen (♛).
2. **To Build:** Go to the **Build** tab. Generate a random board or paint your own. Test it with the **Test Build** button. To play it, click the **Apply To Tabs** button, then go to the **Play** tab. To share it, click the **Share** button and send the puzzle to a friend.
3. **To Learn:** If you get stuck, go to the **Solve** tab. Click **Next Step** to see the logical deduction required to progress.

---

## 📜 License
This project is open-source and available under the **MIT License**.

---

**Built by [Richard Hall](https://www.linkedin.com/in/rilhia/)** 
