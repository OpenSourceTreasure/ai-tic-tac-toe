 ✔ AI Tic Tac Toe

💡 Run Tic-Tac-Toe.html (simple!)

✅ Zero dependencies

✅ Minimax Algorithm guarantees its not easy to win!

🥁 The Minimax algorithm is a decision-making algorithm typically used in game theory for two-player turn-based games like Tic-Tac-Toe, Chess, and Checkers. It works by recursively evaluating all possible moves and selecting the optimal move based on the current state of the game board.

🎷 The algorithm explores all possible board states (all possible moves for both the AI and the player) in a tree-like structure. Each node represents a potential board configuration, and each move corresponds to a branch in the tree.

🎸 The algorithm evaluates all possible moves at each level, choosing the best move for the AI and the best move for the player in the recursive tree. The AI moves to maximize its score, and the player moves to minimize the AI's score.

<p align="center"><img src="https://github.com/OpenSourceTreasure/ai-tic-tac-toe/blob/main/tic-tac-toe.png"></p>


💬 For those interested, here is more detailed info:

Steps of the Minimax Algorithm in the Game:
AI Move: The AI evaluates all possible moves on the board and calculates the best move using Minimax.

Minimax Calculation:

For every empty spot on the board, the AI "places" its symbol (O) and recursively calculates the best possible score.
It then "un-places" the symbol and moves to the next empty spot, continuing the process.
The move with the highest score is chosen as the AI's move.
Player Move: The player chooses a spot, and the AI responds based on the evaluation from Minimax.

Why is Minimax Effective Here?
Optimal Strategy: For Tic-Tac-Toe, which is a small game with a limited number of possible moves, Minimax can evaluate all possible moves in a reasonable amount of time and select the optimal move. This guarantees that the AI never loses and can either win or force a tie, depending on the player's moves.
Tie or Win: Since Tic-Tac-Toe is a solved game, the AI will never lose if it uses the Minimax algorithm correctly.
How It Works in the Game:
In the provided code:

The getBestMove function computes the best possible move using Minimax.
The minimax function evaluates the board recursively, applying the logic described above.
This is a simple AI implementation, and while it works well for a small game like Tic-Tac-Toe, more complex games would require more advanced AI techniques, such as Alpha-Beta Pruning, which optimizes the Minimax algorithm by cutting off branches that don’t need to be explored.
