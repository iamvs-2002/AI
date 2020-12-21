- Bidirectional Search is an extension of BFS or DFS.
- Two simultaneous search from an initial node to goal and backward to from goal to initial, stopping when two meet.
- Each search(2 searches, 1 from each end) covers half of the depth => d/2
- Time Complexity = 2*(b^(d/2))
- Space Cpmplexity = Number of nodes traversed
- Advantage over BFS or DFS: Time complexity is reduced, space complexity remains the same.
- Complete in BFS (Optimal solution is guaranteed).
- Incomplete in DFS (The solution might be Non-Optimal).
- Example:



  
  *               2                   7
  *     1(start)      4     5     6      9(goal)
  *               3                   8

- Example: If we have to reach 9th node, i.e. "goal", then we will start either BFS or DFS from 1 to 9 and simultaneously from 9 to 1
    * That means, the meeting point would be 5
  
