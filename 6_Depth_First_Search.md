- Uninformed Search Technique, i.e., we have only the present knowledge but not the entire domain knowledge.
- Based on the concept of LIFO(last-in-first-out) eg. Stack.
- Works on Deepest Node.
- Example:
  *                    A                      level-0
  *            B              C               level-1
  *         D    E          F   G             level-2
  Now, as we start the process:
   * Stack: A                    
   * Stack: B C
   * Stack: B F G
   * Stack: B F 
   * Stack: B
   * Stack: D E
   * Stack: D
   * **A->C->G->F->B->E->D**
