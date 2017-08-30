Sudoku AI Problem
===

> The task is original by [https://github.com/kwarodom/Sudoku-AI-Problem](https://github.com/kwarodom/Sudoku-AI-Problem)

This is a project that try to solve soduku problem by reduction the problem and using depth first search (DFS) algorithm.

The aiming of solution

1. Remove all possible choices to minimum choices in each cell of sudoku table by remove all candidate which conflict to soduku rules. For example, each row and each column of soduku table must contains only unique nunber.
2. Fill the cell with value which no other cell in corresponding row, column and 3x3 box has the possible choices with the same value. For example, in cell A1...A9, if A1 contains possible choices with 1,3,5 and cell A2...A9 no any possible choices of 1, therefore, A1 is only cell that can fill value with 1.
3. Loop through 1 and 2 approach until there can't reduce possibility to fill sudoku anymore
4. In the case of sudoku can't optimize the possibility to only one choice from 3, the solution will be reduced by searching algorithm called depth first search (DFS). Try to iterate fill the cell with each possible value and recursive to find another possible solutions with this algorithm.

More details and description explained in [solving-a-sudoku-with-ai.ipynb](solving-a-sudoku-with-ai.ipynb)

## Usage

1. Start Docker

```
docker-compose up
```

2. Open website with URL which output from terminal in 1

## License

[MIT](LICENSE) © Kosate Limpongsa