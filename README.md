Tic-Tac-Toe Game

Overview
This is a simple implementation of a Tic-Tac-Toe game using plain JavaScript. 
The game allows two players to take turns and displays a message when a player wins or if the game ends in a draw.

Key Features
Turn-based Gameplay: Alternates turns between Player O and Player X.
Win Detection: Identifies and announces the winner based on predefined win patterns.
Draw Detection: Detects when the game results in a draw after all boxes are filled.
Game Reset: Provides options to reset the game or start a new game.

How It Works
Game State Management: Tracks the current player's turn and the number of moves made.
Win Patterns: Uses a set of win patterns to check for a winning combination.
User Interface: Updates the game board and displays messages for winners or draw scenarios.

Main Functions
resetGame(): Resets the game state, clears the board, and hides the message container.
gameDraw(): Displays a draw message and disables further moves.
disableBoxes(): Disables all game boxes to prevent further input.
enableBoxes(): Enables all game boxes and clears their content.
showWinner(winner): Displays a congratulatory message with the winner's identifier and disables further moves.
checkWinner(): Checks the current board state against predefined win patterns and determines if there is a winner.

Event Listeners
Box Click Event: Handles user input by updating the box content based on the current player's turn, then checks for a winner or draw.
New Game Button: Calls resetGame() to start a new game.
Reset Button: Calls resetGame() to reset the current game state.

Win Patterns
The game uses the following win patterns to determine a winner:

[0, 1, 2] (Top row)
[0, 3, 6] (Left column)
[0, 4, 8] (Diagonal from top-left to bottom-right)
[1, 4, 7] (Middle column)
[2, 5, 8] (Top-right to bottom-right diagonal)
[2, 4, 6] (Top-right to bottom-left diagonal)
[3, 4, 5] (Middle row)
[6, 7, 8] (Bottom row)

Usage
Play: Click on the boxes to place either "O" or "X" based on the current player's turn.
New Game: Click the "New Game" button to reset the game and start a fresh match.
Reset Game: Click the "Reset" button to reset the current game without starting a new one.

