# Godot-GDScript-Objects
Various 2D and 3D programs created using GDScript, a dynamically typed, Python-like programming language for the Godot game engine.

An array based heuristic distance graph algorihm for the Godot game engine's GDScript resides in Shadow3DEnemy-FMA.gd.  It's designed for moving between rooms and then pathing directly to a target.  I originally labeled and intended it to be AStar(), but I was carried away with finishing the project and continued mislabeling the algorithm for about 11 months.  I created a graph of junctions for moving between rooms in a house.   At each iteration, the AI moves to the graph's minimum cost node to get to its moving target (the player or another AI).  The cost of a target is determined by that node's distance from the AI in addition to the goal's heuristic cost calculated as the sum horizontal and vertical distance from the AI to its target.  Rather than using a priority queue and for loop like Djikstra's algorithm, I iterate through a graph of nodes with a heuristic cost factored into distance.  In future games, I will implement an actual A* or experiment with Godot's built in A* functionality.   Why rebuild the wheel?
