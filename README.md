# A* Pathfinding Algorithm Visualizer

This Python script utilizes the Pygame library to implement the A* pathfinding algorithm visualizer. Here's a breakdown of the project:

## Imports

- `pygame`: Required for creating the graphical interface.
- `math`: Used for mathematical calculations.
- `PriorityQueue` from `queue`: Utilized in managing the open set efficiently.

## Global Constants and Initialization

- `WIDTH`: Defines the width of the window.
- `WIN`: Initializes the Pygame display window with the specified width.
- Colors: Defines several color constants used throughout the project.

## Spot Class

Represents each cell or spot on the grid.
- Attributes include position, color, neighbors, and methods for updating and drawing the spot.

## Helper Functions

- `h(p1, p2)`: Calculates the heuristic (Manhattan distance) between two points.
- `reconstruct_path(came_from, current, draw)`: Reconstructs and visualizes the shortest path after the algorithm finishes.
- `make_grid(rows, width)`: Creates a grid of spots based on the number of rows and width.
- `draw_grid(win, rows, width)`: Draws grid lines on the window for visual separation.
- `draw(win, grid, rows, width)`: Updates and draws the grid and spots on the window.
- `get_clicked_pos(pos, rows, width)`: Converts mouse-click positions to grid coordinates.

## Algorithm Implementation

- `algorithm(draw, grid, start, end)`: Implements the A* algorithm using a priority queue for efficient node traversal.

## Main Function

Initializes the grid and handles user interactions such as mouse clicks and key presses.
- Allows the user to create barriers, set the start and end points, visualize the algorithm, and reset the grid.

Overall, the script provides a graphical interface where users can interactively create obstacles, set start and end points, and visualize the A* algorithm finding the shortest path between them on a grid.
