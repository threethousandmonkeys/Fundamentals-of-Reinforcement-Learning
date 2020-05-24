**Lesson 1: The K-Armed Bandit Problem**
* Understand the temporal nature of the bandit problem
  * Samilarity b/w ~ and SUpervised lreaning:
    * the agent does receive some rewards (just like labels in supervised learning)
  * Difference b/w ~ and Supervised learning: 
    * Dataset is not explicitly provided in Bandits with results. Actions are taken and reward is observed
    * there is not necessarily a right or wrong "label" - an action can be rewarding or less rewarding - or not rewarding at all
    * 
* Define k-armed bandit
    * https://blog.csdn.net/pouqiyu5090/article/details/84898609 
    * https://zhuanlan.zhihu.com/p/30822777
* Define action-values
* The value of an action is the expected reward when that action is taken:
* Define reward


**Lesson 2: What to Learn? Estimating Action Values**
* Define action-value estimation methods
* Define exploration and exploitation
* Select actions greedily using an action-value function
* Define online learning
* Understand a simple online sample-average action-value estimation method
* Define the general online update equation
* Understand why we might use a constant stepsize in the case of non-stationarity


**Lesson 3: Exploration vs. Exploitation Tradeoff**
* Compare the short-term benefits of exploitation and the long-term benefits of exploration
* Understand optimistic initial values
* Describe the benefits of optimistic initial values for early exploration
* Explain the criticisms of optimistic initial values
* Describe the upper confidence bound action selection method
* Define optimism in the face of uncertainty
