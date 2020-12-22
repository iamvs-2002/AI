- Heuristic refers to the technique designed to solve a problem quickly.
- Kind of guess work used in Informed Search Approach.
- Rather than exploring every node, we go to the node with the **minimum Heuristic** at the same level.
- To find Heuristic value any of the following method can be used:
  * Eucledian Distance
    * Calculate the distance between two node points (x1,y1) and (x2,y2).
  * Manhattan Distance
    * Used to find verical/horizontal distance, eg. 8 Puzzle Problem.
      * *In 8 Puzzle Problem,  we find Heuristic value by finding the number of missing tiles for each node.*
- Heuristic approach always guarantees the **good solution** but it does not guarantee the optimal solution.
- In an average case, it is better in terms of time as compared to Blind Search/ Uninformed Search
