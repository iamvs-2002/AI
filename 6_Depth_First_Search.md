- Uninformed Search Technique, i.e., we have only the present knowledge but not the entire domain knowledge.
- Based on the concept of LIFO(last-in-first-out) eg. Stack.
- Works on Deepest Node.
- Incomplete.
- Possibility exists that it doesn't give us a result, if there are cycles are in the graph or the depth is infinite(i.e. search space is infinite).
- Might give non-optimal solution.
- Time Complexity = O(V+E)
   * V = no. of nodes
   * E = no. of edges
- Time Complexity = O(b^d)
   * b = branch factor
   * d = depth

- Example:
  *                    A                      level-0
  *            B              C               level-1
  *         D    E          F   G             level-2
  Now, as we start the process:
   * Stack: A                    
   * Stack: B C
   * Stack: B F G
   * Stack: B F 
   * Stack: B
   * Stack: D E
   * Stack: D
   * **A->C->G->F->B->E->D**
   * Example: If we want to find G, the route is: A->C->G as per the above process
