- Agent can be anything: a human, a program or a machine.
- Operations performed by an agent:
  * It percepts the environment through the sensors.
  * Then based on the perceptions, it takes some actions with the help of Agent Programs.
  * Agent Programs are used to decide the action by relating it to some past event.
  * Actuator is used to take the actions.
  * The output is given through the Effectors.
  * This output causes some change in the environment.
  * Agent -> Percept -> Decision(Agent Program) -> Actions(Output)
- 
- Goals:
  * High Performance
  * Optimized Result
  * Rational Action
-   
- Factors behind the model of any agent:
  * **P** : Performace
    * eg. It should ensure safety, comfortness etc.
  * **E** : Environment
  * **A** : Actions
  * **S** : Sensors
- 
- Types of Agents:
  * **Simple Reflex Agents**
    * Acts only on the basis of **current perception**.
    * Takes immediate action without any calculation.
    * Ignores the rest of the percept history(knowledge gained in the past).
    * **Based on If/then rules => condition statements.**
    * Environment should be **fully observable**(agent should be knowledgeable about the whole environment).
    * Environment -> Percept(through sensors) -> Current Situation(of environment) -> If/then(condition) -> Takes action(through actuator) -> Change in Environment
    * eg. If temperature>45 degree, switch on the AC.
  * **Model Based Reflex Agents**
    * Acts on the basis of **current perception + history/past**.
    * Knowledge based agent(past events).
    * **Partially observable** environment.
    * Environment -> Percept(through sensors) -> Current Situation(of environment) -> Save the state(temporarily) -> Relate to past events -> If/then(condition) -> Takes               action(based on those past events)(through actuator) -> Change in Environment
    * **Store Percept History(Internal Model).**
  * **Goal Based Agents**
    * Expansion of Model Based Reflex Agents.
    * Based on **Desirable Situation**(Goal).
    * Example of supervised learning.
    * This technique is based on **Searching** and **Planning**.
    * Environment -> Percept(through sensors) -> Current Situation(of environment) -> Save the state(temporarily) -> Relate to past events -> If/then(condition) -> Thinks of           different possible actions and their effects -> Thinks of best action to achieve the **goal** -> Takes action(based on those past events)(through actuator) -> Change in         Environment
  * **Utility Based Agents**
    * **Focus on utility, not goal**.
    * It depends on the effect of an action on the state of the agent: happy or unhappy state
    * Utility function is used to measure the happiness or unhapiness of the sate after an action has been performed.
    * Environment -> Percept(through sensors) -> Current Situation(of environment) -> Save the state(temporarily) -> Relate to past events -> If/then(condition) -> Thinks of           different possible actions and their effects -> Thinks of how happy is the state after the action has been performed -> Takes action(based on those past events)(through actuator) -> Change in Environment
  * **Learning Agents**



