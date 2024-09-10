# PRODIGY_SD_04
# Sudoku Solver

This project is a Python implementation of a Sudoku solver that automatically solves Sudoku puzzles using the backtracking algorithm. The program can take any unsolved Sudoku grid as input and fill in the missing numbers to complete the puzzle.

## How It Works

The Sudoku Solver uses a backtracking algorithm, a depth-first search technique, to find the correct numbers for each empty cell in the grid. Here's a brief explanation of the process:

1. **Grid Representation**: The Sudoku puzzle is represented as a 9x9 grid, where empty cells are denoted by `0`.
2. **Finding Empty Cells**: The solver scans the grid to find the first empty cell.
3. **Validation**: For each empty cell, the algorithm checks whether a number from 1 to 9 can be placed without violating Sudoku rules (i.e., the number should not already exist in the same row, column, or 3x3 subgrid).
4. **Backtracking**: The algorithm attempts to fill each empty cell with a valid number. If it encounters a conflict, it backtracks to the previous cell and tries the next possible number.
5. **Solution**: The process continues until the grid is fully and correctly filled, or it determines that no solution exists.

## Features

- Solves standard 9x9 Sudoku puzzles.
- Displays the grid before and after solving.
- Efficiently uses backtracking to find the solution.
- Easy to modify for other grid inputs.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/sudoku-solver.git
   ```

2. Navigate to the project directory:

   ```bash
   cd sudoku-solver
   ```

3. Run the solver:

   ```bash
   python sudoku_solver.py
   ```

4. Modify the `sudoku_grid` variable in the code with your own puzzle to solve.

## Example

### Input (Unsolved Sudoku Grid)

```plaintext
5 3 . . 7 . . . .
6 . . 1 9 5 . . .
. 9 8 . . . . 6 .
8 . . . 6 . . . 3
4 . . 8 . 3 . . 1
7 . . . 2 . . . 6
. 6 . . . . 2 8 .
. . . 4 1 9 . . 5
. . . . 8 . . 7 9
```

### Output (Solved Sudoku Grid)

```plaintext
5 3 4 6 7 8 9 1 2
6 7 2 1 9 5 3 4 8
1 9 8 3 4 2 5 6 7
8 5 9 7 6 1 4 2 3
4 2 6 8 5 3 7 9 1
7 1 3 9 2 4 8 5 6
9 6 1 5 3 7 2 8 4
2 8 7 4 1 9 6 3 5
3 4 5 2 8 6 1 7 9
```

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests if you have suggestions or improvements.

