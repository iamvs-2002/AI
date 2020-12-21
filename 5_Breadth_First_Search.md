- Uninformed Search Technique, i.e., we do not have any domain specific knowledge.
- Based on FIFO(first-in-first-out) eg. Queue
- Also called as Level Search Technique because it moves level by level.
- Shallowest node
- Complete
- Optimal solution is guaranteed.
- Time complexity
- Example:


    *                           A                        level - 0
    *                B          C         D              level - 1
    *           E    F        G    H      I              level - 2
    *      J    K             L           M              level - 3
    *           N                                        level - 4
    
    Now, as we start making the queue, 
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
