# 🎮 The Shuffle Game - Turbo C++ Puzzle

A classic number sliding puzzle implemented using **Turbo C++ graphics**. This is a terminal-based game where the user needs to arrange numbers in ascending order by moving tiles using keyboard input.

---

## 🧠 Game Objective

Arrange the shuffled numbers from **1 to 8** in ascending order on a **3x3 board**, leaving one tile blank.

```
Initial (Shuffled):        Final (Goal):
+---+---+---+               +---+---+---+
| 5 | 3 | 8 |               | 1 | 2 | 3 |
+---+---+---+               +---+---+---+
|   | 2 | 4 |     --->      | 4 | 5 | 6 |
+---+---+---+               +---+---+---+
| 1 | 6 | 7 |               | 7 | 8 |   |
+---+---+---+               +---+---+---+
```

---

## 📂 File Structure

```
/ShuffleGame
│
├── SHUFFLEG.CPP     # Main Turbo C++ Source Code
└── README.md        # Project documentation
```

---

## 🧰 Technologies Used

- **Turbo C++ Graphics**
- `<graphics.h>`, `<conio.h>`, `<stdio.h>`, `<stdlib.h>`, `<string.h>`
- Classic DOS interface

---

## 🕹️ How to Play

1. Use Turbo C++ (TC3) to compile and run the program.
2. When prompted:
   - Press `1` to start the game.
   - Press `2` to read the rules.
3. Use **keyboard number keys (1–8)** to move a number tile.
4. Keep sliding until all numbers are in ascending order.
5. Press **X** anytime to exit the game.

---

## 📝 Features

- Intro animation with credits
- Menu interface with instructions
- Movement counter
- Valid move checker (prevents invalid moves)
- Victory screen with congratulations
- Max moves limit (80) for challenge

---

## ⚙️ Compilation & Run (Turbo C++ only)

### 📦 Requirements

- Turbo C++ IDE (DOS-based)
- DOSBox (for modern systems)

### ▶️ Steps

1. Open **Turbo C++**
2. Load `SHUFFLEG.CPP`
3. Compile: `Alt + F9`
4. Run: `Ctrl + F9`

Ensure the BGI folder path is set correctly:
```cpp
initgraph(&gdriver, &gmode, "c:\\turboc3\\bgi");
```

---

## 🧠 Game Logic

- `initial()` – Initializes numbers randomly
- `check()` – Validates if a move is allowed
- `userwin()` – Checks if the player has arranged all tiles correctly
- `easy()` – Main game loop with drawing, input, and step counter
- `draw()` – Displays individual number tiles using ASCII box format

---

## 🎯 Winning Condition

The game is won when the `num[]` array contains numbers in this sequence:

```
[1, 2, 3, 4, 5, 6, 7, 8, 0]
```

Where `0` represents the blank tile.

---

## 🧱 Limitations

- **Turbo C++ specific**: Requires DOSBox or legacy environment.
- No support for mouse input or modern graphics.
- Limited to static shuffle pattern, not fully randomized.

---

## 💡 Future Improvements

- Port to modern C++ with SDL or SFML
- Add randomized puzzle generator
- Add score leaderboard
- GUI version with mouse/touch support

---

## 👤 Credits

Developed by: **Shlok Verma**  
Language: **Turbo C++**  
Project Type: **Mini Project / Console Puzzle Game**

---

## 📜 License

Free to use, modify, and learn from!  
Distributed under the **MIT License**
