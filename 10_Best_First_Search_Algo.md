- Informed, Heuristic method
- Greedy for the heuristic value(min)
- It guarantees the good solution but it might give non-optimal solution.
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


