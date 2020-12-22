- Informed, Heuristic method
- Greedy for the heuristic value(min)
- **Here we do not take care about the cost, but only the minimum heuristic value.**
- It guarantees the good solution but it might give non-optimal solution.
- In an average case, Time Complexity is less than the uninformed searching.
- In the worst case, the Time Complexity = O(b^d)
  * b = branch factor
  * d = depth
- Here we explore the node with the minimum heuristic value while keeping other nodes in the memory(priority queue).
  * Hence, the space complexity becomes infinite as all the nodes are kept in the memory/priority queue.
- After the elements have been added at the end of the queue, we sort(ascending) them according to their heuristic value
- Algorithm:
  * Let 'OPEN' be a priority queue containing the initial state.         //priority is based on the heuristic value of that node
  * Loop
    * if OPEN is empty return failure
    * Node <- Remove-First(OPEN)      //else remove the first node from the OPEN, that is called a Node
      * if Node is a Goal
      * then return the Path from initial to Node
    * else generate all the successors of the Node and
    * Put the newly generated Node into OPEN
    * according to their f values(heuristic value)
  * END Loop
- Complete Algorithm because it takes all the elements in the priority queue and hence ensures the optimal solution.

