## Running the Code on Google Colab

To run the Python script (.py file) on Google Colab, follow these steps:

1. *Open Google Colab:*
   - Go to [Google Colab](https://colab.research.google.com/).

2. *Create a New Notebook:*
   - Click on File in the menu.
   - Select New notebook to create a new Colab notebook.

3. *Upload the Python Script:*
   - In the Colab notebook, click on the Files icon on the left sidebar (a folder icon).
   - Click on Upload and select the .py file from your local machine.

4. *Run the Python Script:*
   - Copy the code from the uploaded python file into a code cell and run to get the output


# OptimalPathFinding

The A* algorithm is a widely used pathfinding algorithm in computer science and artificial intelligence. It is an informed search algorithm that efficiently finds the shortest path between two points on a graph or grid. A* combines the advantages of Dijkstra's algorithm (guaranteed shortest path) and greedy best-first search (efficiency) by using a heuristic to guide its search.

A* selects nodes from the open list with the lowest combined cost (actual cost + heuristic) for expansion, gradually moving towards the goal node. By intelligently prioritizing nodes to explore, A* can efficiently find the optimal path while avoiding unnecessary exploration of less promising paths.

One key feature of A* is its optimality and completeness under certain conditions, ensuring that it will always find the shortest path if one exists. However, the performance of A* heavily depends on the quality of the heuristic function used. A well-designed heuristic can significantly improve search efficiency by guiding A* towards the goal more effectively.

Program Components
1. Class Definitions:
- `Cell`: Represents a single cell in the grid. Each cell has attributes for its coordinates (`x`, `y`) and whether it is traversable.
- `Grid`: Initializes a grid of cells with a specified width and height. It also includes functions to manipulate individual cells, such as setting them as obstacles or checking their traversability status.
2. Distance Calculation:
- `euclidean_distance`: Computes the Euclidean distance between two points in a two-dimensional space. It utilizes the Pythagorean theorem to calculate the distance between pairs of coordinates.
3. A* Search Algorithm:
- `a_star`: Performs the A* search algorithm to find the optimal path from a starting cell to a goal cell on the grid. It manages an open set as a priority queue to evaluate nodes based on their estimated total cost (`f_score`). The algorithm iterates through neighboring cells, updates the path if a better route is found, and adds unvisited neighbors to the open set until the goal cell is discovered.
4. Neighborhood Generation:
- `get_neighbors`: Generates neighboring cells that are traversable and within the grid boundaries. It searches for cells in the cardinal directions (left, right, top, bottom) relative to the given cell.
5. Path Reconstruction:
- `reconstruct_path`: Reconstructs the optimal path from the `came_from` dictionary generated during A* search. It traces the parent cells backward from the goal cell to the starting cell.
6. Graphical User Interface (GUI):
- `main`: Creates an interactive GUI using IPywidgets for users to input grid dimensions, add obstacles, set start and goal positions, and visualize the pathfinding process. When the visualize button is clicked, the grid, obstacles, start, goal, and optimal path are displayed using Matplotlib.

Outputs

![image](https://github.com/user-attachments/assets/01f766eb-f470-44a1-ae79-5e798f064205)

![image](https://github.com/user-attachments/assets/fb7d8a43-b307-4ccf-b39b-e5fabe3bf4e4)
