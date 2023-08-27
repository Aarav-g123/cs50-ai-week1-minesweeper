## Minesweeper AI using Propositional Logic and Knowledge-based Agents

This program, `minesweeper.py`, implements an AI player for the game Minesweeper using propositional logic and knowledge-based agents. The AI makes inferences about the locations of mines and safe cells based on the revealed cells and the number of neighboring mines. The AI employs a set of logical sentences to represent its knowledge about the game board.

### Requirements

Before running the program, make sure you have the required packages installed. You can install them using the following command:

```bash
pip install -r requirements.txt
```

### How to Run

To use the Minesweeper AI, you can follow these steps:

1. Make sure you have Python and the required packages installed.
2. Open a terminal window and navigate to the directory containing `minesweeper.py` and `requirements.txt`.
3. Install the required packages using the command mentioned above.
4. Run the AI by executing the following command:

```bash
python minesweeper.py
```

The AI will start playing Minesweeper on an 8x8 grid by default. You can modify the grid size or other parameters within the `MinesweeperAI` class.

### License

This program is provided under the MIT License

### How the AI Works

The Minesweeper AI uses a knowledge-based approach to make inferences about the game board. It maintains a set of logical sentences, each representing the relationship between certain cells and the count of neighboring mines. The AI follows these steps during its gameplay:

1. **Initialization**: The Minesweeper game board is represented by the `Minesweeper` class, and the AI logic is implemented in the `MinesweeperAI` class.

2. **Gameplay Loop**: The AI iterates through a loop of moves, making decisions based on its current knowledge.

3. **Adding Knowledge**: When the AI receives information about a safe cell and the count of neighboring mines, it updates its knowledge base using the `add_knowledge` method. This method adds new sentences and uses existing knowledge to make inferences about safe cells and mines.

4. **Making Safe Moves**: The AI employs the `make_safe_move` method to determine the next safe move. This method selects a safe cell that has not been chosen before.

5. **Making Random Moves**: If no known safe moves are available, the AI uses the `make_random_move` method to select a random move that is neither a known mine nor a previously chosen cell.

6. **Inference and Logic**: The AI's knowledge base includes logical sentences that represent constraints on mine placement. It uses deduction and inference to identify safe cells and mine locations based on the constraints.

### Note

This program aims to demonstrate a basic implementation of a Minesweeper AI using propositional logic and knowledge-based agents. It may not cover all possible game scenarios or advanced strategies.

For more sophisticated Minesweeper AI implementations, additional optimization and strategy development might be required.
