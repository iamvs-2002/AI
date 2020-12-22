- Backtracking algorithm.
  * It means that we move from root to the terminal level and calculate the values using which we again propagate to the root level and then we decide which move to choose.
- Best move strategy is used.
  * It means each player/opponent tries to play hi best move to win,i.e., to stop the opponent from winning.
- In game playing, Breadth First Search Technique is not used because it works level by level.
- Max will try to maximize utility(Best move).
- Min will try to minimize utility(Worst move).
- Time Complexity = O(b^d)
  * b = branch factor(i.e. choices)
  * d = depth/ply
- Minimax Method can be used only in some games but not in every game because the search tree in some games(eg. chess) will be very vast and hence time complexity will be           infinite. To bring some efficiency, we use α-β pruning method.
