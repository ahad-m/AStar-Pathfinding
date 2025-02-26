# A* Pathfinding Algorithm with Visualization

This project implements the A* pathfinding algorithm, designed to find the shortest path in a grid-based environment while avoiding obstacles. The algorithm is visualized using a simple graphical user interface (GUI), where users can see the grid, obstacles, pathfinding process, and f(n) values.

## Project Overview

The A* algorithm uses a heuristic to make informed decisions, allowing it to efficiently navigate through a grid to reach a goal while avoiding obstacles. This project includes the following components:

- **AStar.java**: The core A* pathfinding algorithm.
- **Grid.java**: A class that represents the grid, manages obstacles, and provides neighbors for the pathfinding algorithm.
- **AStarGUI.java**: A GUI to visualize the grid, obstacles, and the pathfinding process, displaying useful information like f(n) values.

## Files Explanation

### AStar.java
Contains the implementation of the A* algorithm:
- `aStar(Grid grid, Node start, Node goal)`: Main function that performs the A* search.
- `calculateHeuristic(Node node, Node goal)`: Calculates the heuristic (Octile Distance) for the algorithm.
- `reconstructPath(Node current)`: Reconstructs the path from goal to start.

### Grid.java
Defines the grid and its obstacles:
- `generateRandomObstacles(int obstacleCount)`: Generates random obstacles on the grid.
- `isObstacle(int x, int y)`: Checks if a specific position is an obstacle.
- `getNeighbors(Node node)`: Retrieves valid neighboring nodes of a given node.

### AStarGUI.java
Provides a graphical user interface to visualize the pathfinding process:
- Draws the grid and updates the grid with obstacles, the start, goal, and the found path.
- Displays path length, f(n) values, and total path cost.
- Includes a "Start" button to trigger the pathfinding process.
