# Nim Game AI

This is an implementation of the Nim game along with an AI player that uses Q-learning to learn and improve its gameplay over time.

## Game Rules

Nim is a two-player mathematical game where players take turns removing objects (such as stones) from distinct piles. The game starts with several piles, each containing a specific number of objects. On their turn, a player must choose one pile and remove one or more objects from it. The player who takes the last object(s) from the last pile wins the game.

## How to Run

To play the game against the AI or train the AI, you can execute the `main.py` file. Make sure you have Python 3 installed on your system.

```bash
python main.py
```

## Classes

### Nim

The `Nim` class represents the Nim game. It keeps track of the game state, including the number of objects in each pile, the current player, and the winner. The class provides methods for making moves, switching players, and checking for a winner.

### NimAI

The `NimAI` class represents the AI player in the Nim game. It uses Q-learning to learn and improve its gameplay. The AI maintains a Q-learning dictionary that maps state-action pairs to Q-values. It provides methods for updating the Q-values based on rewards, selecting the best action to take, and choosing actions with exploration (epsilon-greedy strategy).

### Training

The `train` function trains the AI by playing multiple games against itself. It initializes an instance of the `NimAI` class and plays the specified number of games. After each move, it updates the AI's Q-values based on the rewards received. The function returns the trained AI.

### Playing

The `play` function allows a human player to play against the AI. It creates an instance of the `Nim` game and alternates turns between the human player and the AI. The function prompts the human player for their moves and uses the AI to make its moves. It displays the game state after each move and determines the winner at the end of the game.

## Dependencies

The code does not have any external dependencies beyond Python 3.

## License

This code is licensed under the MIT License. You can find the full license text in the `LICENSE` file.

Feel free to modify and use the code according to your needs.

## Acknowledgments

This code is based on the Nim game and Q-learning concepts. The implementation is inspired by various resources and tutorials on game AI and reinforcement learning.
