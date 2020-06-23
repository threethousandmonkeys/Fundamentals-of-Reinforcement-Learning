## Module 01: Monte Carlo Methods for Prediction & Control 
#### Lesson 1: Introduction to Monte Carlo Methods 
* Understand how Monte-Carlo methods can be used to estimate value functions from sampled interaction
  * MC methods estimate values by **averaging** over a large number of **random samples**.
  * 采样越多，找到的解越接近最优解 => As the number of samples increases, the average tends to get closer and closer to the expected return.
  * ![image](IMG/MC_algo.png)
  The Monte Carlo algorithm has to keep track of multiple observed returns
  * 
* Identify problems that can be solved using Monte-Carlo methods




* Use Monte Carlo prediction to estimate the value function for a given policy. 


#### Lesson 2: Monte Carlo for Control 
* Estimate action-value functions using Monte Carlo
* Understand the importance of maintaining exploration in Monte Carlo algorithms 
* Understand how to use monte carlo methods to implement a GPI algorithm. 
* Apply Monte Carlo with exploring starts to solve an MDP 

#### Lesson 3: Exploration Methods for Monte Carlo 
* Understand why Exploring Starts can be problematic in real problems 
* Describe an alternative exploration method for Monte Carlo control 

#### Lesson 4: Off-policy learning for prediction 
* Understand how off-policy learning can help deal with the exploration problem 
* Produce examples of target policies and examples of behavior policies.
* Understand importance sampling
* Use importance sampling to estimate the expected value of a target distribution using samples from a different distribution. 
* Understand how to use importance sampling to correct returns
* Understand how to modify the monte carlo prediction algorithm for off-policy learning. 