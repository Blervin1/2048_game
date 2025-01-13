# 2048 Game Implementation

Welcome to the **2048 Game**! This project is a JavaScript-based implementation of the popular sliding tile puzzle game. Test your skills as you merge tiles to reach the elusive 2048 tile. 🚀

---

## [DEMO](https://Blervin1.github.io/2048_game/)

## 🎯 Goal

Combine tiles on a 4x4 grid by sliding them in four directions (up, down, left, right). When two tiles with the same value collide, they merge into one. Reach a tile with the value **2048** to win the game!

But beware — the game ends when there are no more valid moves left. Good luck, ninja! 🥷

---

## 📂 Project Structure

This project consists of two main components:

### 1. **Game Logic**

The game logic is written in the `src/modules/Game.class.js` file, which includes the core functionality of the game. The `Game` class has several methods you need to implement.

#### Obligatory Methods:

- `constructor(initialState = null)`: Initializes the game board.
- `getState()`: Returns the current game board state.
- `getScore()`: Returns the current score.
- `getStatus()`: Returns the game status (`playing`, `won`, or `lost`).
- `moveLeft()`, `moveRight()`, `moveUp()`, `moveDown()`: Moves the tiles in the respective direction and updates the board.
- `start()`: Starts the game and displays the board.
- `restart()`: Resets the game to the initial state.

### 2. **Game UI**

The UI is built using the `src/index.html` and `src/main.js` files. It leverages the `Game` class to manage the game logic and updates the DOM to reflect the game state.

---

## 📜 Rules

1. **Grid**: The game is played on a 4x4 grid.
2. **Numbers**: Each cell is either empty or contains a number (2, 4, 8, ...).
3. **Movement**: Use the arrow keys to slide tiles in the desired direction.
4. **Merging**: Tiles with the same value merge into one and double their value.
5. **Random Tiles**: After each move, a random empty cell will receive a 2 or 4 (4 appears with 10% probability).
6. **Winning Condition**: If any tile reaches 2048, you win!
7. **Game Over**: The game ends if there are no more valid moves.
8. **Score**: Your score increases by the sum of all merged tiles in a move.

---

## 🛠️ How to Play

1. Clone this repository:
   ```bash
   git clone https://github.com/Blervin1/2048-game.git
   cd 2048-game
   npm install
   npm run start
   ```
2. Use the arrow keys to move tiles and try to reach 2048.

## 💡 Tips

**Focus on larger tiles:** Merge smaller tiles into larger ones to make progress faster.

**Plan ahead:** Avoid moves that isolate high-value tiles in corners.

**Practice:** The more you play, the better you'll get at strategizing!

## 🎨 Styling

Each tile has a dynamic class: `field-cell--%cell_value% (e.g., field-cell--2, field-cell--4)`.
Use the hidden class to toggle visibility for elements like start and restart buttons.
Change the button's style dynamically using `start` and `restart` classes.

## 📜 License

`This project is licensed under the MIT License. Feel free to use, modify, and share it as you like.`
