- Informed Searching, Heuristic
- * here means admissible, i.e., A* algorithm guarantees the optimal solution.
- f(N) = g(N) + h(N)
  * f(N) = Cost
  * g(N) = Actual cost from the start node to n(intermediate node)
  * h(N) = Estimation of the cost(heuristic value) from n to the Goal node
- We calculate f(N) for each node in the graph/tree and move along with the one having minimum f(N).

