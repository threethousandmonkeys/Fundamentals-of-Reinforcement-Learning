**Lesson 1: Policy Evaluation (Prediction)**
* Understand the distinction between policy evaluation and control
  * Policy evaluation is the task of determining the value function for a specific policy. Policy evaluation is the task of determining the state value function v pi for a particular policy pi.
  * Control is the task of finding a policy to obtain as much reward as possible. In other words, **finding a policy which maximizes the value function.** Control is the ultimate goal of reinforcement learning.
  * The goal of the control task is to modify a policy to produce a new one which is strictly better.Control is the task of improving an existing policy.
* Explain the setting in which dynamic programming can be applied, as well as its limitations
  * Dynamic programming uses the various Bellman equations we've seen, along with knowledge of p, to work out value functions and optimal policies. Classical dynamic programming does not involve interaction with the environment at all. Instead, we use dynamic programming methods to compute value functions and optimal policies given a model of the MDP.
  *  dynamic programming is very useful for understanding other reinforced learning algorithms. Most reinforced learning algorithms can be seen as an approximation to dynamic programming without the model.


* Outline the **iterative policy evaluation** algorithm for estimating state values under a given policy
  * we have a procedure we can apply to iteratively refine our estimate of the value function.
* Apply iterative policy evaluation to compute value functions

**Lesson 2: Policy Iteration (Control)**
* Understand the **policy improvement theorem**
  * the policy improvement theorem tells us that greedified pi policy is a strict improvement, unless the original policy was already optimal.
  * ![image](/IMG/policy_improvement_theorem.png)
  * Policy Pi prime is at least as good as Pi if in each state, the value of the action selected by Pi prime is greater than or equal to the value of the action selected by Pi. Policy pi prime is strictly better if the value is strictly greater and at least one state. 
* Use a value function for a policy to produce a better policy for a given MDP
* Outline the policy iteration algorithm for finding the optimal policy
  * Evalueation and Improvement 
  * Deterministic ->  Each policy generated in this way is deterministic. There are finite number of deterministic policies, so this iterative improvement must eventually reach an optimal policy.
* Understand “the dance of policy and value”, how policy iteration reaches the optimal policy by alternating between evaluating policy and improving it,
  * ![image](/IMG/policy_interation.png)
  * We can visualize this dance as bouncing back and forth between one line, where the value function is accurate, and another where the policy is greedy. These two lines intersect only at the optimal policy and value function. Policy iteration always makes progress towards the intersection by projecting first onto the line v equals v Pi, and then onto the line where Pi is greedy with respect to v. Of course, the real geometry of the space of policies and value functions is more complicated, but the same intuition holds.
  * ![image](/IMG/policy_iter_code.png)
* Apply policy iteration to compute optimal policies and optimal value functions

**Lesson 3: Generalized Policy Iteration**
* Understand the framework of generalized policy iteration
* Outline value iteration, an important example of generalized policy iteration
Understand the distinction between synchronous and asynchronous dynamic programming methods
* Describe brute force search as an alternative method for searching for an optimal policy
* Describe Monte Carlo as an alternative method for learning a value function
* Understand the advantage of Dynamic programming and “bootstrapping” over these alternative strategies for finding the optimal policy