- Local search algorithm,i.e., it has the knowledge of its local domain but not of the global domain.
- Here Beam Width(β) = 1
- Greedy approach.
  * Works till it gets the best move.
  * Once it gets the best move, it stops.
- No backtracking(if it doesn't find the best move).
- Algorithm:
  * Evaluate the initial state
  * Loop until a solution is found or there are no operators left
  * Select and apply a anew operator
  * Evaluate the new state:
      * if goal, then quit
      * if better than current state(i.e., heuristic value of the new state less than that of the current state), then it is new current state
