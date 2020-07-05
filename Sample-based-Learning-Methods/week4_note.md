## Module 3: emporal Difference Learning Methods for Prediction & Temporal Difference Learning Methods for Control 

### Lesson 1: TD for Control 
* Explain how generalized policy iteration can be used with TD to find improved policies 
  * Monte Carlo methods wait until the return following the visit is known, then use that return as a target for V (St)
    * V (St) <-  V (St) + α[G_t - V (St)], where Gt is the actual return following time t, and α is a constant step-size parameter
* Describe the Sarsa Control algorithm
* Understand how the Sarsa control algorithm operates in an example MDP
* Analyze the performance of a learning algorithm 


### Lesson 2: Off-policy TD Control: Q-learning 
* Describe the Q-learning algorithm
* Explain the relationship between q-learning and the Bellman optimality equations. 
* Apply q-learning to an MDP to find the optimal policy
* Understand how Q-learning performs in an example MDPUnderstand the differences between Q-learning and Sarsa
* Understand how Q-learning can be off-policy without using importance sampling 
* Describe how the on-policy nature of SARSA and the off-policy nature of Q-learning affect their relative performance 


### Lesson 3: Expected Sarsa 
* Describe the Expected Sarsa algorithm
* Describe Expected Sarsa’s behaviour in an example MDP
* Understand how Expected Sarsa compares to Sarsa control
* Understand how Expected Sarsa can do off-policy learning without using importance sampling
* Explain how Expected Sarsa generalizes Q-learning 