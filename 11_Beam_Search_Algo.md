- An extension of Best First Search Algorithm.
- Takes care of Space Complexity(constant).
- Beam Width(β) is given.
- In Best First Search Algorithm, we keep all the elements in the priority queue.
- In Beam Search Algorithm, we keep only some elements in the priority queue(*after sorting*) as per the beam width.
    * If beam width is 2, we keep the best 2 elements in the priority queue.
    * This way the space complexity is reduced.
    * Because of the beam width search, the space complexity becomes constant.
- Just like Best First Search Algorithm, here we take care only of the minimum heuristic value and not about the cost of the action.
