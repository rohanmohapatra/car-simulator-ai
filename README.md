# car-simulator-ai
Car Simulator-Artificial Intelligence - UE16CS325
 
CAR SIMULATOR
Pranav Pahwa- 01FB16ECS265
Rhythm Girdhar- 01FB16ECS302
Rohan B Sahu- 01FB16ECS305
Rohan Mohapatra- 01FB16ECS307
Problem Statement
Visualisation of A* search algorithm to effectively find the solution to the path-finding problem in a static- obstacle car simulation application. 
Introduction
The Car simulation application uses the A* search algorithm to find the shortest possible path from the user-defined start state to the goal state (user-defined) while considering all the blocked paths, manually provided by the user. The project has been extended with a choice of heuristics to be applied along with the different modes of displaying the optimal path. 
Why A* search?
The most important problem is choosing the most adequate path-finding algorithm.  The A* algorithm provides an effective solution to the problem of pathfinding and it also be one of the most popular algorithm used for the game’s development. Assuming a path exists between the starting point and the ending point; then the A* algorithm guarantees to find the best path.
A* search is:
Complete
Optimal
Optimally Efficient
Also, The most interesting applications of A* search are in games. Hence, applying this search algorithm was a perfect choice as we were using a small-scale problem where any of its drawbacks of space inefficiency are not affecting us. 
Goals
Developing a game environment where a car can be simulated from the given start state to goal state. 
Implementation of one of the best searching algorithms known in Artificial Intelligence- A* search. 
Integrating algorithmic approach with real-world graphics.  
Learning the basic decision making which is essential for domains like Computer Vision. 
Specifications
Technical Approach
Language used: Python 2.6
Libraries used:  PyGame
Milestones
Initial benchmark
Usage of Pygame to develop a basic structure of the game where the best path is obtained, using the basic heuristic functions. 
Final Presentation
Accurate code for all the different types of displays for optimal path as well for different types of heuristic functions.  
Integration of graphics to display the movement of car, along with the optimal path. 
Algorithm- A* search
A* Search algorithm is one of the best and popular technique used in path-finding and graph traversals.
A* algorithm is a best-first search algorithm in which the cost associated with a node is :
 f(n) = g(n) + h(n),
where g(n) = cost of the path from the initial state to node n
           h(n) = heuristic estimate or the cost or a path from node n to a goal
Thus, f(n) estimates the lowest total cost of any solution path going through node n. At each point a node with lowest f value is chosen for expansion.
A* algorithm guides an optimal path to a goal if the heuristic function h(n) is admissible, meaning it never overestimates actual cost. It expands the fewest number of nodes.
The main drawback of A* algorithm and indeed of any best-first search is its memory requirement. Since at least the entire open list must be saved, A* algorithm is severely space-limited in practice.
Details
Heuristics used:
Manhattan: It is the sum of absolute values of differences in the goal’s x and y coordinates and the current cell’s x and y coordinates respectively, i.e.,
h = abs (current_cell.x – goal.x) + abs (current_cell.y – goal.y)
Straight line distance:  It is the distance between the current cell and the goal cell using the distance formula
	h = sqrt ( (current_cell.x – goal.x)2 + (current_cell.y – goal.y)2 )
      3.   Zero (Nothing Known)- No heuristic  
Modes for displaying the optimal path:
Verbose
Instant
Steps through Path
How to use the simulation?
Install Python 2.6 and PyGame to execute. 

Command
Commands.txt
Code
Car_path.py
Future Enhancements
The simulation environment will be made dynamic i.e the obstacles will be added at the run-time and will not be predefined by the player/user.
Scaling the project up by integrating the concepts of Image Processing from Machine Learning and Neural Networks. 
Conclusion
Hence, while developing the game, we learnt about a python library called Pygame which is extremely useful in game development in terms of useful modules for algorithms as well as graphics. 
The project also helped us in understanding the real- life applications of various search algorithms, taught us during the course. It worked as a motivation to enhance our project to apply other domains of artificial intelligence and learn more about the subject in detail.

  Literature Survey
Introduction to A* search http://theory.stanford.edu/~amitp/GameProgramming/AStarComparison.html
PyGame Documentation
https://www.pygame.org/docs/
Simulating Car Racing Game by Applying Pathfinding Algorithms http://www.ijmlc.org/papers/82-A1090.pdf
Heuristics 
http://theory.stanford.edu/~amitp/GameProgramming/Heuristics.html
pygame.Surface documentation
https://www.pygame.org/docs/ref/surface.html
