- Backtracking algorithm.
  * It means that we move from root to the terminal level and calculate the values using which we again propagate to the root level and then we decide which move to choose.
- Best move strategy is used.
  * It means each player/opponent tries to play hi best move to win,i.e., to stop the opponent from winning.
- Since this is a backtracking based algorithm, it tries all possible moves, then backtracks and makes a decision.
- In game playing, Breadth First Search Technique is not used because it works level by level.
- Max will try to maximize utility(Best move).
- Min will try to minimize utility(Worst move).
- Time Complexity = O(b^d)
  * b = branch factor(i.e. choices)
  * d = depth/ply
- Minimax Method can be used only in some games but not in every game because the search tree in some games(eg. chess) will be very vast and hence time complexity will be           infinite. To bring some efficiency, we use α-β pruning method.
- Here we are maximizing player.
- Example:
  * <img src="https://media.geeksforgeeks.org/wp-content/uploads/minmax.png"/>
  * Maximizer goes LEFT: It is now the minimizers turn. The minimizer now has a choice between 3 and 5. Being the minimizer it will definitely choose the least among both,i.e., 3
  * Maximizer goes RIGHT: It is now the minimizers turn. The minimizer now has a choice between 2 and 9. He will choose 2 as it is the least among the two values.
  * Being the maximizer you would choose the larger value that is 3. Hence the optimal move for the maximizer is to go LEFT and the optimal value is 3.
  * Now the search tree becomes:
  * <img src = "https://media.geeksforgeeks.org/wp-content/uploads/minmax1.png"/>
