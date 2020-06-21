## Lesson 1: Policies and Value Functions

* Recognize that a policy is **a distribution over actions for each possible state**
![image](/IMG/policy.png)
  *  π(S) represents the action selected in state S by the policy π. In this example, π selects the action A1 in state S0 and action A0 in states S1 and S2. 
  *  We can visualize a deterministic policy with a table. Each row describes the action chosen by π in each state. 
  *  the agent can select the same action in multiple states, and some actions might not be selected in any state. 


* Describe the similarities and differences between stochastic and deterministic policies
  *  Deterministic policy -> a policy maps each state to a single action.
  *  A stochastic policy is one where multiple actions may be selected with non-zero probability.
     *  might choose "up" or "right" in their decision making.


* Identify the characteristics of a well-defined policy
  * Policies can only depend on the current state.
* Generate examples of valid policies for a given MDP
  ![image](/IMG/valid&notvalid.png)
The sceond one would not be a valid policy because this is conditional on the last action. That means the action depends on something other than the state. 

* Describe the roles of state-value and action-value functions in reinforcement learning
  * a state value function is the future award an agent can expect to receive starting from a particular state. More precisely, the state value function is the expected return from a given state.
  ![image](/IMG/state-value.png)
  * An action value describes what happens when the agent first selects a particular action. More formally, the action value of a state is the expected return if the agent selects action A and then follows policy Pi. 
![image](/IMG/action-value.png)

* Describe the **relationship between value functions and policies**
  * Value function enable us to judge the quality of different policies.
  *  State-value functions represent the **expected return** from a given state under a specific policy.
  * Action value functions represent the **expected return** from a given state after taking a specific action, later following a specific policy.  
* Create examples of valid value functions for a given MDP
  * Chess game

## Lesson 2: Bellman Equations

* Derive the Bellman equation for state-value functions
![image](/IMG/state_bellman.png) 


* Derive the Bellman equation for action-value functions
![image](/IMG/action_bellman.png)

* The current time-step's state/action values can be written recursively in terms of future state/action values.
* Understand how Bellman equations **relate current and future values**
* Use the Bellman equations to compute value functions

## Lesson 3: Optimality (Optimal Policies & Value Functions)

* Define an optimal policy
  * -> the policy with the highset possible value function in all states.
  * One policy is better than another? -> We will say policy Pi one is as good as or better than policy Pi two, if and only if the value under Pi one is greater than or equal to the value under Pi two for **every state**. 只要有一个 就不能说是greater。
  * But we can have an extra state π3, which is combine the two policies and always choose the better one in a state.
* Understand how a policy can be at least as good as every other policy in every state
  * At lease one optimal policy always exists, but there may be more than one.
* Identify an optimal policy for given MDPs
  * depends on Gamma - γ
  ![image](/IMG/policy_on_MDP.png)
  But we can only solve small MDPs, if we have a general MDP, the number of possible policies will be a very large number, then we cannot use brute-force search. -> but we can use **bellman optimality equations.**

* Derive the Bellman optimality equation for state-value functions
* Derive the Bellman optimality equation for action-value functions
![image](/IMG/bellman-optimal-state:action.png)
* Understand how the Bellman optimality equations relate to the previously introduced Bellman equations
  * the Bellman equations form a linear system of equations that can be solved by standard methods. The Bellman's optimality equation gives us a similar system of equations for the optimal value.
  * but we cannot slove bellman optimality equation as bellman quations since the MAX is non linear.

* Understand the connection between the optimal value function and optimal policies
* Verify the optimal value function for given MDPs