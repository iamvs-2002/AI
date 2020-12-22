- Local search algorithm,i.e., it has the knowledge of its local domain but not of the global domain.
- Here Beam Width(β) = 1.
- Space complexity is reduced as β = 1.
- Greedy approach.
  * Works till it gets the best move.
  * Once it gets the best move, it stops.
- **No backtracking**(if it doesn't find the best move).
- Algorithm:
  * Evaluate the initial state
  * Loop until a solution is found or there are no operators left
  * Select and apply a anew operator
  * Evaluate the new state:
      * if goal, then quit
      * if better than current state(i.e., heuristic value of the new state less than that of the current state), then it is new current state
- Problems in Hill Climbing Algorithm:
 * Local Maximum
   * If their is some other state which is better than the current state and the intermediate state between that state and the current state is not a better state as compared to        the current state, the algorithm will stop and hence, we will not reach the optimal solution.
     * Example: In the x-y graph is their exist two local maximas, M1 and M2 and M2>M1.
       * If we have arrived at M1, the algorithm will stop because just after M1 their is a local minimum. Hill CLimbing Algo rithm only moves if the new state is better than            the current state.
       * i.e., the local maximum is achieved but not the global maximum.
     * Example: In the 8 puzzle problem if all the new states have a heuristic value greater than that of the current state, the Hill Climbing Algorithm will stop on the current          state, which might not be the optimal/best solution(i.e., the goal state).
 *
