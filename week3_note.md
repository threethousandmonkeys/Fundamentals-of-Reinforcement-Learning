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
  * Stae-value functions represent the **expected return **from a given state under a specific policy.
  * Action value functions represent the **expected return** from a given state after taking a specific action, later following a specific policy.  


* Describe the **relationship between value functions and policies**
* Create examples of valid value functions for a given MDP
  * Chess game

## Lesson 2: Bellman Equations

* Derive the Bellman equation for state-value functions
* Derive the Bellman equation for action-value functions
* Understand how Bellman equations relate current and future values
* Use the Bellman equations to compute value functions

## Lesson 3: Optimality (Optimal Policies & Value Functions)

* Define an optimal policy
* Understand how a policy can be at least as good as every other policy in every state
* Identify an optimal policy for given MDPs
* Derive the Bellman optimality equation for state-value functions
* Derive the Bellman optimality equation for action-value functions
* Understand how the Bellman optimality equations relate to the previously introduced Bellman equations
* Understand the connection between the optimal value function and optimal policies
* Verify the optimal value function for given MDPs