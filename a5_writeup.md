# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

DFS takes longer as it tries a lot more combinations, while DFS is quicker but uses more memory. If someone wants an optimal solution to a problem BFS would be good, however if memory is limited then DFS would be good.

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

Stack I believe is the most recent element added is the first to be removed or changed. Queue I believe is the first element added is the first to be removed or changed. Some alternative data structures that I researched is a deque or a priority stack.

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

The Sudoku solver can be extended to different games such as checkers. The sudoku solver uses a lot of recursion to deduce if they made a good move that solves the board, and if altered a little bit it could potentially look at all the possible moves on a checker board and deduce which is the best move. This can be applied to real world problem solving as many problems need to be solved by backtracking and finding previous mistakes or clues. So when solving real world problems instead of just looking towards the future we can also backtrack to solve the problem.
