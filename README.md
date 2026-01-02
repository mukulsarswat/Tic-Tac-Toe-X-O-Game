# 🎮 Tic Tac Toe Game in C++

A simple **console-based Tic Tac Toe game** implemented in C++ with colorful text output and cross-platform support for keyboard input.

---

## ✨ Features
- **Cross-platform input handling**  
  - Uses `conio.h` for Windows  
  - Uses `termios` for Linux/Unix (custom `getch()` implementation)

- **Colored text output** using ANSI escape codes for better visualization.

- **Player name input**: Prompts both players to enter their names before starting.

- **Dynamic board rendering**: Displays the Tic Tac Toe grid after every move.

- **Win detection**: Checks rows, columns, and diagonals for a winner.

- **Draw detection**: Declares a draw if all 9 cells are filled without a winner.

- **Replay option**: Players can restart the game without exiting the program.

---

## 🛠️ How It Works
1. **Main Menu**  
   - Option `1`: Start the game  
   - Option `2`: Exit  

2. **Player Setup**  
   - Enter names for Player 1 (`X`) and Player 2 (`O`).

3. **Gameplay**  
   - Players press keys `1–9` to mark their moves.  
   - Board updates after each move.  
   - Colors distinguish between `X` (Red) and `O` (Blue).

4. **Win/Draw Check**  
   - Game checks after each move for a winning combination.  
   - Highlights winning cells in **Green**.  
   - Declares draw if no winner after 9 moves.

5. **Restart Menu**  
   - Option `1`: Replay with same players.  
   - Option `2`: Exit the game.

---

## 📂 Code Structure
- **Text Color Functions**: `red()`, `Blue()`, `Green()`, etc. for colored output.
- **Class `ticTacToe`**  
  - `inputPalyerName()` → Get player names  
  - `setDataTicTacArray()` → Initialize board  
  - `printData()` → Display board  
  - `userInput()` → Handle player moves  
  - `checkElement()` → Validate and place moves  
  - `checkWiningGame()` → Detect winner  
  - `displayResult()` → Show final board with highlights  
  - `restartGame()` → Replay or exit  
  - `mainMune()` → Main menu loop  

---

## ▶️ Compilation & Execution
```bash
# Compile
g++ ticTacToe.cpp -o ticTacToe

# Run
./ticTacToe
