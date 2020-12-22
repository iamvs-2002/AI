- Informed Searching, Heuristic
- "star" here means admissible, i.e., A* algorithm guarantees the optimal solution but only in underestimation case.
- f(N) = g(N) + h(N)
  * f(N) = Cost
  * g(N) = Actual cost from the start node to n(intermediate node)
  * h(N) = Estimation of the cost(heuristic value) from n to the Goal node
- We calculate f(N) for each node in the graph/tree and move along with the one having minimum f(N).
- Time Complexity = O(V+E)
  * V = Number of nodes
  * E = Number of edges
- Time Complexity = O(b^d)
  * b = branch factor
  * d = depth
- Space Complexity = O(b^d)

- 
- h(N) : heuristic value/estimated value of the cost from n to the Goal node
- h*(N) : actual value of the cost from n to the Goal node
-    h(N) <= h*(N)  :   Underestimation
-    h(N) >= h*(N)  :   Overestimation
- **Underestimation guarantees the optimal solution whereas Overestimation does not guarantee the optimal solution.**
- In case of Underestimation:
  * If f(Goal Node) is less than the node(other way from the start node than which we chose), then it will stop and give the optimal solution.
  * If f(Goal Node) is more than the node(other way from the start node than which we chose), then it will not stop and will go to that node to reach the goal state and hence give     the optimal solution.
