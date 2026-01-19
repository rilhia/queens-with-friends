![Main Header Logo](images/QueensWithFriendsLogo.png)

# Queens With Friends ♛
> **Play, challenge, and learn logic with friends.**

**Queens With Friends** is an open-source logic puzzle engine. Unlike competitive leaderboards that can be manipulated by scripts, this platform is a transparent environment for true enthusiasts to sharpen their minds, build their own challenges, and learn the deep logic behind every move.

---

## 🏁 Quick Start: I Just Want to Play!
<img src="images/screenshot1.png" width="300">

When you first load the game, a puzzle is already waiting for you on the **Play** tab.

1.  **Start the Game:** Press the "Start Game" button. A 3-2-1 countdown will begin to get you ready.
2.  **Marking Blocks (•):** Touch a cell once to mark it as blocked. You can also swipe your finger across several cells to block them all at once.
3.  **Setting a Queen (♛):** Double-tap a cell to place a queen.
4.  **Removing Pieces:** To unblock a cell or remove a queen, simply touch it again.
5.  **Tracking Progress:** Every move you make is recorded in the activity log below the board.

> ⚠️ **Important:** If you leave the **Play** tab to look at other sections during a game, the board will reset. Make sure to finish your solve before switching tabs!

---

## 🎮 The Rules
<img src="images/screenshot2.png" width="300">

The goal is to place exactly **one queen** in every row, every column, and every color region. To win, you must satisfy four constraints:

1.  **Row:** Exactly one queen per row.
2.  **Column:** Exactly one queen per column.
3.  **Region:** Exactly one queen per color-coded region.
4.  **Adjacency:** Queens cannot touch each other, not even diagonally.

---

## 🛠️ The Build Tab: Customize Your Challenge
The **Build** tab is the heart of the engine. Here you can load pre-made boards, generate random puzzles, or architect your own.

### 1. Loading Pre-Made Levels
<img src="images/screenshot3.png" width="300">

We have included a library of curated boards that are guaranteed to have a unique solution.
* Select your **Size** (from 5x5 up to 10x10).
* Select your **Difficulty** (Easy, Medium, Hard, or Super Hard).
* Choose a board from the **Load Board** dropdown.
* Once selected, click the **Apply to Tabs** button to send it to the Play and Solve tabs.

### 2. Generating Random Puzzles
* Select your desired size and difficulty, then click **Generate Random**.
* **Small boards (5x5):** These generate in just a few seconds.
* **Large boards (10x10):** High-difficulty large boards are mathematically complex and can take several minutes to compute.
* **Verification:** Once a board is found, you must click **Test Build** to verify it. Once you see the success message, click **Apply to Tabs**.

### 3. Manual Design (Painting Your Own)
<img src="images/screenshot4.png" width="300">

* Flip the **Manual Edit** switch to see the color palette appear.
* Pick a color and tap cells on the board to "paint" custom regions.
* **Test Your Architecture:** Click **Test Build** to see if your design is valid. 
* **Show Solutions:** Tick the "Show Solutions" box before clicking **Test Build**. The engine will show you exactly where queens can be placed on your custom layout—this is incredibly helpful for adjusting your design!

---

## ✉️ Sharing Challenges
Once you have a verified board, you can challenge your friends:

* **The Share Button:** On mobile, this opens your device's sharing options. On desktop, it copies a unique URL to your clipboard. This link contains the entire board state—your friend just clicks it and starts playing.
* **Manual Text Import:** Below the buttons is a text area containing the board code (e.g., `[[0,0...]]`). You can copy this text manually. To load it, your friend simply pastes it into their text box and hits **Test Build**.

---

## 💡 The Solve Tab: Learn the Logic
<img src="images/screenshot5.png" width="300">

The **Solve** tab is designed to teach you *how* to think. 

1.  Apply a board from the Build tab.
2.  Click **Next Step** to watch the engine solve the puzzle one move at a time.
3.  **The Reasoning Log:** Every move includes a detailed explanation of the logic used (such as **Super-Intersections**, **Mutual Exclusion**, or **Contradiction Chaining**).
4.  Use this tab on harder boards to learn advanced techniques that you can then apply to your own manual solves.

---

## 🛡️ The Mission
This project returns "Queens" to its roots as a pure logic exercise.
1.  **P2P Challenges:** Competition happens between friends via direct links, not an anonymous leaderboard.
2.  **Educational Focus:** The built-in solver exposes the "why" behind every deduction.
3.  **Creative Freedom:** Users are encouraged to build and validate their own puzzles to share.

---

## 🛠️ Technical Implementation
* **Greedy Snakes Algorithm:** A custom procedural generator for organic region growth.
* **Heuristic Deduction Engine:** A multi-layered solver that mimics human logic patterns.
* **Zero-Server P2P:** Entire board states are stored in **Base64 URL Encoding**, requiring no databases or accounts.

**Built by [Richard Hall](https://www.linkedin.com/in/rilhia/)** | **[MIT License](https://opensource.org/licenses/MIT)**
