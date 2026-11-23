# ❌⭕ Terminal Tic-Tac-Toe: A Python Logic Game

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mayen-Shahriar-Kabir/Terminal_Tic-Tac-Toe/blob/main/<Insert-File-Name>.ipynb)

A modular, terminal-based Tic-Tac-Toe game built entirely in Python. This project is open-sourced as a pedagogical tool to help computer science students transition from basic scripts to state-managed applications using 2D data structures and algorithmic win-checking.

You can play the game instantly in your browser by clicking the **Open in Colab** badge above.

### 🎮 How to Play
1. Run the code cell in Google Colab.
2. Player 1 is assigned 'X' and Player 2 is assigned 'O'.
3. The board is numbered 1 through 9. When prompted, enter the number corresponding to the grid slot where you want to place your character.
4. The game will automatically alternate turns, clear the terminal output for a clean UI, and declare a winner or a draw after 9 inputs.

### 🧑‍🏫 Pedagogical Value (For Beginners)
This codebase serves as an excellent foundational case study for introductory programming concepts. By reviewing the code, students can explore:

* **2D Data Structures:** The game board is managed using a nested list (matrix) `[[1,2,3],[4,5,6],[7,8,9]]` to represent the grid.
* **Algorithmic Logic:** Win conditions are broken down into dedicated, modular functions: `checkHorizontal()`, `checkVertical()`, and `checkDiagonal()`.
* **State Management & Game Loops:** A central `runGame()` function utilizes a `while` loop bound by `totalInputs = 9` to manage the turn-based state, track valid moves, and detect draw conditions.
* **Advanced Input Mapping:** User inputs (1-9) are mapped to their exact 2D list coordinates (e.g., `5` becomes `[1, 1]`) using a dictionary named `pos_to_board_index`.
* **Data Validation:** The code checks the ASCII values of the board slots using `ord()` in the range 49-57 to ensure players cannot overwrite an existing 'X' or 'O'.
* **Clean UI Execution:** The `IPython.display.clear_output` function is used sequentially to refresh the board state without cluttering the terminal history.
