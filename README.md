TicTacToe 🎮

A classic, interactive Tic Tac Toe game built from scratch using HTML, CSS, and vanilla JavaScript. 

![Tic Tac Toe Preview](excited.gif) <!-- You can replace this with a screenshot of your actual game later -->

## 🚀 Functionality & Features
* **Interactive Gameplay**: Playable 2-player game on a single screen.
* **Win Validation**: Automatically detects when a player gets 3 in a row (horizontally, vertically, or diagonally).
* **Audio Effects**: Includes sound effects for making a move, winning the game, and background background music to enhance the experience.
* **Visual Feedback**: 
  * A dynamic strike-through line appears across the winning combination.
  * An animated GIF pops up to celebrate the winner.
* **Reset mechanism**: A dedicated reset button allows players to instantly clear the board and start a new match without refreshing the page.

## 🛠️ How it Works

### How the Game Begins
1. The game starts with an empty 3x3 grid.
2. By default, **Player 'X'** always goes first.
3. The info panel on the right side of the board indicates whose turn it is. 

### Gameplay Loop
1. Players take turns clicking on empty boxes on the grid.
2. The JavaScript logic ensures a box cannot be overwritten once a move is made.
3. Every time a move is played, the [changeTurn()]function swaps the active player from 'X' to '0' (or vice versa) and an audio chime is triggered.

### How the Game Ends
1. After every move, the [checkWin()] function scans the board against an array of 8 possible winning combinations.
2. If a match is found:
   * The text in the info panel announces the winner (e.g., "X Won").
   * A purple line transforms and rotates across the winning boxes.
   * A celebratory animated GIF expands into view.
   * Further clicks on the board are disabled until the game is reset.
3. Players can click the **Reset** button at any time to clear the grid, hide the line and GIF, and restart the game with 'X's turn.

## 🎨 Styling & Design
* **Layout**: Built using **CSS Flexbox** for overall page layout and **CSS Grid** (`grid-template-rows`, `grid-template-columns`) specifically to construct the perfectly proportioned 3x3 game board.
* **Custom Fonts**: Typography uses clean Google Fonts (`Roboto` for the UI and `Baloo Bhaina 2` for the game info).
* **Classic Board Look**: Specific borders were selectively removed (via classes like `.br-0`, `.bt-0`) to give the grid the classic "hashtag" shape rather than looking like a spreadsheet table.
* **Responsive Design**: Includes a CSS media query that triggers at screens under `950px` wide, wrapping the layout so the board sits cleanly above the game info on smaller devices like tablets and mobile phones.
* **Smooth Transitions**: CSS transitions are used for hover effects on the board squares and for smoothly animating the winning line and celebration GIF.

## 💻 Tech Stack
* **HTML5**: Semantic structure.
* **CSS3**: Layout, Flexbox, CSS Grid, and responsive design.
* **JavaScript**: DOM manipulation, event listeners, array methods, and game logic.


