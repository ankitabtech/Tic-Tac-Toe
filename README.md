# Tic-Tac-Toe


The provided Java code implements a simple console-based Tic-Tac-Toe game for two players (X and O). The game uses a 3x3 board, and players take turns making moves until one player wins or the game ends in a draw. The program checks for wins by rows, columns, and diagonals. It also validates moves and prevents players from making moves on already occupied positions. The game continues until a player wins or a draw occurs.

Key Points:

Board Representation: The game board is represented as a 3x3 array of characters (board), initialized with empty spaces.

Player Turns: Players take turns making moves, starting with 'X'. The currentPlayer variable is used to keep track of the current player, and it switches between 'X' and 'O' after each move.

User Input: The program uses a Scanner to get user input for row and column numbers to make a move.

Move Validation: The isValidMove method checks if the entered move is within the valid range and if the selected position on the board is unoccupied.

Making Moves: The makeMove method updates the board with the current player's symbol at the specified row and column.

Switching Players: The switchPlayer method toggles between 'X' and 'O' for the next move.

Winning Conditions: The checkWin method checks for wins by calling separate methods (checkRows, checkColumns, checkDiagonals) to examine rows, columns, and diagonals.

Checking Rows and Columns: The checkRows and checkColumns methods iterate through rows and columns, respectively, to find three consecutive symbols in a line.

Checking Diagonals: The checkDiagonals method checks both main and anti-diagonals for a win.

Draw Condition: The checkDraw method checks if there are no empty spaces left on the board, indicating a draw.

Printing the Board: The printBoard method displays the current state of the board after each move.

Game Loop: The game runs in an infinite loop until a player wins or the game ends in a draw. The loop breaks when either condition is met.

Console Output: The program outputs messages for each player's turn, invalid moves, a winning player, or a draw.

Resource Management: The Scanner is closed at the end of the game to release resources.
