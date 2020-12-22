- Based on AND/OR Graph.
- Works on the basis of Problem Decomposition(breakdown of complex problem into smaller problems).
- Informed Searh Technique.
- A* always gives the optimal solution while AO* does not explore all the solution paths once it gets the solution.
- Example:
  *                          A
  *             6B     x    12C        10D
  *          5G   7H                 4E  x 4F
  * Here, x represents the hyper edge((B and C),(E and F)) and 6,12 etc are the heuristic values(estimation values)
  * The cost of each edge = 1
  *
  * Total cost when we go from A -> B,C = 6+12+1+1 = 20
  * Total cost when we go from A -> D = 10+1 = 11
  * Since 11 is less than 20, we chose the path: A -> D
  * Total cost when we go from D -> E,F = 1+1+4+4 = 10 = revised cost = heuristic value of D
  * Hence, total cost at A = 11
  * Now, since it got the solution, it will stop without even exploring on the other path, i.e., from A->B,C which might give the optimal solution.
  * Here, we first find the heuristic value of each node level by level and on reaching the end, we update those heuristic values as per the the heuristic value of the final node     and hence we get the solution graph.
- Steps:
  * Step-1: Create an initial graph with a single node (start node).
  * Step-2: Transverse the graph following the current path, accumulating node that has not yet been expanded or solved. 
  * Step-3: Select any of these nodes and explore it. If it has no successors then call this value- FUTILITY else calculate f'(n) for each of the successors.
  * Step-4: If f'(n)=0, then mark the node as SOLVED.
  * Step-5: Change the value of f'(n) for the newly created node to reflect its successors by backpropagation.
  * Step-6: Whenever possible use the most promising routes, If a node is marked as SOLVED then mark the parent node as SOLVED.
  * Step-7: If the starting node is SOLVED or value is greater than FUTILITY then stop else repeat from Step-2.
