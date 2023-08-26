# de_dust2-pathfinding
This was a project for my Master's. It includes pre-prossecing on the Counter Strike: Global Offensive map de_dust2 followed by multiple pathfinding algorithms.

The first step was importing the map and transforming it to an occupancy grid map (OGM). Then BrushFire algorithm was used to help us with the next step.

The second step was equipping the map with a uniform probabilistic road map (PRM) and a random one. After this the pathfinding algorithm where use on random point on the map.

Step three, Dijkstra and A* are executed on the PRMs and plotted showing the searched area (red lines) by the algorithm and the final path it found (blue dots). Every step of the algorithms can be seen by a single tweak in the code.

Step four, rapidly-expanding random trees (RRT) and rapidly-expanding random trees star (RRT*) were used straight on the OGM to connect the goal with the start node. As in the previous step area visited and found path can be seen on the plots.

Lastly, path smoothing is applied in every path found by the algorithms with care, so none of the points end up outside the bound of the map.