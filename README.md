AI Project: 8-Puzzle Game Solver Using A Algorithm*
This project implements the 8-Puzzle Game using the A* search algorithm to find the optimal solution to reach the goal state from a given starting state. The 8-puzzle is a classic problem in artificial intelligence where the goal is to arrange the tiles in a specific order by sliding them into the empty space.

Project Overview
The 8-puzzle consists of a 3x3 grid, with eight numbered tiles and one empty space. The task is to slide the tiles around until the puzzle is solved, i.e., the tiles are arranged in a defined order. This project uses the A* search algorithm, which is an informed search technique, to efficiently solve the puzzle.

The A* algorithm is used to explore possible moves, with the goal of finding the sequence of moves that leads to the solved state in the least number of steps.

Key Features
A* Algorithm: The main search strategy used to find the optimal solution.
Heuristic Function: The heuristic used is the Manhattan distance, which calculates the total number of moves required to bring each tile to its correct position.
State Space Representation: The state of the puzzle is represented as a 3x3 grid, and the program tracks the current state and previous states during the search.
Visualization: The current state of the puzzle is displayed after each move, showing how the tiles are moved to reach the goal state.
How the A* Algorithm Works
Initial State: The starting configuration of the 8-puzzle.
Goal State: The desired configuration (usually ordered tiles 1 to 8 with an empty space).
Heuristic Function: The heuristic function calculates the Manhattan distance for each tile, which helps guide the algorithm towards the goal.
Cost Function: The cost is determined by the number of moves from the initial state, which the algorithm minimizes.
Search: The algorithm explores neighboring states by sliding tiles into the empty space and selects the path that minimizes the total cost (actual path cost + estimated cost to the goal).
Project Structure
puzzle.py: Contains the main implementation of the A* algorithm and the game logic for solving the puzzle.
solver.py: Handles the logic for running the A* search, including state transitions and managing the open and closed lists.
visualizer.py: Optional file for displaying the puzzle at each step of the solution.
test_cases.py: Contains a set of predefined test cases to evaluate the performance and correctness of the A* algorithm.
Technologies Used
Python: The programming language used for implementing the algorithm and puzzle solver.
A* Algorithm: The search algorithm used to solve the puzzle optimally.
Manhattan Distance: The heuristic used to guide the A* search.
Project Dependencies
numpy: Used for matrix operations and manipulation of puzzle states.
heapq: Used for efficient priority queue management (for A* algorithm).
Conclusion
This project demonstrates the application of the A* search algorithm to solve the 8-puzzle game efficiently. The algorithm uses the Manhattan distance heuristic to minimize the number of moves required to solve the puzzle. Through this project, we showcase how AI techniques can be applied to solve classic problems and optimize decision-making processes.
