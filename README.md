# Optimized-TicTacToe-AI
This project implements an AI that plays Tic-Tac-Toe optimally using the Minimax algorithm. The goal is to create an unbeatable AI for the classic game, ensuring that it never loses when played against a human opponent or another AI. The project consists of two main files: runner.py and tictactoe.py.

tictactoe.py: Contains all the game logic, including the implementation of the Minimax algorithm to determine the optimal move at each step.
runner.py: Provides a graphical interface to play the game. Once all functions in tictactoe.py are correctly implemented, you can run this file to play against the AI.
Project Details
Game Representation

The Tic-Tac-Toe board is represented as a list of three lists (3x3 grid), where each cell contains one of three possible values: X, O, or EMPTY.
The game starts with the board in its initial state, and the AI decides the best moves based on the current board configuration.
Function Implementations

To create the AI, the following functions are implemented in tictactoe.py:

player(board): Determines which player's turn it is (X or O) based on the current board state.
actions(board): Returns a set of all possible moves (i.e., empty cells) that can be taken on the current board.
result(board, action): Returns the new board state that results from applying the specified action (move) without modifying the original board.
winner(board): Checks the board and returns the winner (X or O) if there is one, otherwise returns None.
terminal(board): Determines if the game is over, either due to a win or a tie.
utility(board): Returns the utility value of a terminal board: 1 if X wins, -1 if O wins, and 0 for a tie.
minimax(board): Implements the Minimax algorithm to calculate the optimal move for the current player (X or O) on the board. If the board is in a terminal state, the function returns None.
How It Works
Initialization: The game begins with an empty board, and players take turns making moves.
Minimax Algorithm: The AI uses Minimax to evaluate all possible outcomes of each move and chooses the one that maximizes its chances of winning (or minimizes its chances of losing, depending on the player).
Game Play: After implementing the logic in tictactoe.py, run python runner.py to play against the AI in a graphical interface. The AI will always make the optimal move, ensuring that it never loses.
Features
Unbeatable AI: The AI uses Minimax, a decision rule for minimizing the possible loss in a worst-case scenario, ensuring optimal play.
Graphical Interface: Easily test and play against the AI using the provided graphical interface.
Educational: Learn how to apply search algorithms like Minimax in game theory and AI development.
