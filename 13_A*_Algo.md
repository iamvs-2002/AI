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
  * If f(Goal Node) is more than the node(other way from the start node than which we chose), then it will not stop and will go to that node to reach the goal state and hence give     the optimal solution.
- A* Algorithm is one of the best path finding algorithms.
- But it does not produce the shortest path always because it heavily depends on heuristics.
- 
- Steps:
1. Put the initial node in a list OPEN.
2. If (OPEN is empty) or (OPEN=GOAL) then terminate search.
3. Else remove the first node from OPEN. Call this node a.
4. If (a=GOAL) then terminate with SUCCESS.
5. Else if node a has successors, generate all of them. Estimate the f(n) of all of them and sort the list by fitness number, i.e., by f(n).
6. Name the new list is CLOSED.
7. Replace OPEN with CLOSED.
8. Go to step 2.
