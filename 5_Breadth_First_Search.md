- Uninformed Search Technique, i.e., we do not have any domain specific knowledge.
- Based on FIFO(first-in-first-out) eg. Queue.
- Also called as Level Search Technique because it moves level by level.
- Works on Shallowest node.
- Complete
- Optimal solution is guaranteed, i.e., it gives the shortest cost.
- Time complexity = O(V+E)
     * V = no. of nodes
     * E = no. of edges
- Time complexity = O(b^d)
     * b = branch factor(maximum children of a particular node)
     * d = depth
- Space Cpmplexity = Number of nodes traversed
- Example:


    *                           A                        level - 0
    *                B          C         D              level - 1
    *           E    F        G    H      I              level - 2
    *      J    K             L           M              level - 3
    *           N                                        level - 4
    
    Now, as we start the process, 
    * Queue: A
    * Queue: B C D
    * Queue: C D E F
    * Queue: D E F G H 
    * Queue: E F G H I
    * Queue: F G H I J K
    * Queue: G H I J K
    * Queue: H I J K L
    * Queue: I J K L
    * Queue: J K L M
    * Queue: K L M
    * Queue: L M N
    * Queue: M N
    * Queue: N

    * Example: If we want to find G, b = 3 and d = 2
        * Therefore, Time complexity = O(b^d) = 3^2 = 9
        * That means, at max. 9 searches will be required for finding G in the above tree iff the cose at each edge is same.
- In case of 8 Puzzle Problem, b is found using the average case = (4x3 + 4x2 + 4x1)/(3x3) = 2.6.. = 3
