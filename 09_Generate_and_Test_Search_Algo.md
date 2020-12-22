- Heuristic Technique //Informed Search Technique
- It uses DFS with backtracking
- Works in 2 modules: Generate and Test.
- We generate all the possible solutions which are tested by the test module.
- If the goal state is achieved, the solution is accepted, else the solution is dropped.

- So basically it has 3 steps:
  * Generate a possible solution.
  * Test if this solution is the actual solution.
  * If the solution is found, quit, else go back to step 1.
  
- Properties of Good Generators/Good heuristic:
  * Complete, i.e., it will definitely give a possible solution by covering all the states.
  * Non redundant, i.e., we try to reduce the redundant(repeating) states.
  * Informed.
