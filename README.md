# python-tic-tac-toe
A simple two-player Tic-Tac-Toe game built with Python using functions, lists, loops, and conditional logic.


# 🎮 Python Tic-Tac-Toe

A simple **two-player Tic-Tac-Toe game** built using Python. The game runs in the terminal and allows two players to take turns placing **X** and **O** on a 3×3 board.

This project was created to practice fundamental Python programming concepts such as functions, lists, loops, conditional statements, user input, and game-state validation.

## ✨ Features

* 🎮 Two-player gameplay
* ❌ Player 1 uses **X**
* ⭕ Player 2 uses **O**
* 🧩 3×3 Tic-Tac-Toe board
* 🔄 Alternating player turns
* 🏆 Automatic winner detection
* 🤝 Automatic draw detection
* 🚫 Prevents players from selecting an occupied space
* 💻 Runs directly in the terminal

## 🛠️ Technologies Used

* **Python 3**
* Lists
* Functions
* Conditional statements
* Loops
* User input
* Boolean logic

## 🎯 How to Play

The game board contains 9 positions:

```text
| 1 | 2 | 3 |
| 4 | 5 | 6 |
| 7 | 8 | 9 |
```

Players take turns entering a number from **1 to 9** corresponding to the position where they want to place their symbol.

For example:

```text
Your turn player1
Enter your move (1-9): 5
```

The selected position will be marked with the player's symbol.

The first player to get **three matching symbols in a row, column, or diagonal** wins.

If all nine spaces are filled without a winner, the game ends in a draw.

## 🚀 Getting Started

### Prerequisites

Make sure Python 3 is installed on your system.

Check your Python version:

```bash
python --version
```

or:

```bash
python3 --version
```

### Installation

Clone this repository:

```bash
git clone https://github.com/your-username/python-tic-tac-toe.git
```

Move into the project directory:

```bash
cd python-tic-tac-toe
```

### Run the Game

Run the Python file:

```bash
python tic_tac_toe.py
```

## 📂 Project Structure

```text
python-tic-tac-toe/
│
├── tic_tac_toe.py
└── README.md
```

## 🧠 How the Code Works

### 1. Board Initialization

The game board is represented using a Python list containing 9 empty positions.

```python
board = ["  " for i in range(9)]
```

Each index represents one position on the Tic-Tac-Toe board.

### 2. Displaying the Board

The `print_board()` function formats the list into a 3×3 game board and displays it in the terminal.

### 3. Player Movement

The `player_move()` function:

* Identifies the current player.
* Takes the player's move as input.
* Checks whether the selected position is available.
* Places the player's symbol on the board.

### 4. Checking for a Winner

The `is_victory()` function checks all possible winning combinations:

* Three rows
* Three columns
* Two diagonals

If the same symbol occupies one of these combinations, the function returns `True`.

### 5. Checking for a Draw

The `is_draw()` function checks whether all board positions have been filled without a winner.

### 6. Main Game Loop

The `while True` loop controls the overall game:

1. Display the board.
2. Player X makes a move.
3. Check whether X has won.
4. Check whether the game is a draw.
5. Player O makes a move.
6. Check whether O has won.
7. Continue until there is a winner or draw.

## 📌 Python Concepts Practiced

This project helped practice:

* Variables
* Lists
* `for` loops
* `while` loops
* Functions
* `if/elif/else`
* Boolean expressions
* Logical operators
* String formatting
* User input
* Indexing
* Game-state management

## 🔮 Future Improvements

Possible improvements for future versions:

* Add input validation for invalid entries.
* Prevent crashes when users enter letters instead of numbers.
* Allow players to restart the game without rerunning the program.
* Add a single-player mode against a computer.
* Add difficulty levels.
* Keep track of player scores.
* Improve the terminal interface with colors and formatting.
* Create a graphical version using Tkinter or Pygame.

## 👩‍💻 Author

**Manchal Gupta**

This project was developed as part of my journey in learning and strengthening Python programming fundamentals.
