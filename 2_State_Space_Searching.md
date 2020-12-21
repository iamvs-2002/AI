In AI, we majorly talk about how to represent the problem **precisely** and hence **analyse** it.

To represent the problem in all set of states, we use **State Space Searching**.

S : { S , A , Action(S) , Result(S,A) , Cost(S,A) }

* **S** : Set of all possible states: start, intermediate, goal
* **A** : Set of all possible actions
* **Action(S)** : The chosen action from the set of all actions
* **Result(S,A)** : The resulting states formed after any action is performed
* **Cost(S,A)** : The cost paid after a particular action is performed (for example, in searching, the cost of searching should be less)

The action which has the minimum cost is opted.
