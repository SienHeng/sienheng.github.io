---
permalink: /
title:
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi, I am Sien Heng, a freshman undergraduate student at [Department of Mathematics](https://www-math.umd.edu/) of the [University of Maryland](https://umd.edu/).

Some of my academic interests are

* High dimensional inferencing
* Statistical decision making (Reinforcement learning, etc)
* Machine learning theory
* Optimization
* Stochastic processes

During my free time, I like to do some readings, playing billiard, and running.


# My favourite mathematical function
 - The AIXI Function, a theoretical model of an optimal decision-making agent, as known as Artificial General Intelligence(AGI), defined by Marcus Hutter in 2000, the mathematical representation is as follows:

$$
a_t := \arg\max_{a_t} \sum_{e_t r_t} \dots \max_{a_m} \sum_{e_m r_m} [r_t + \dots + r_m] \sum_{q:U(q, a_1 \dots a_m)=e_1 r_1 \dots e_m r_m} 2^{-\text{len}(q)}
$$

 - The AIXI equation defines an optimal agent by choosing actions that maximize expected future rewards based on all possible computable universes.

* **$$a_t$$**: The **action** taken by the agent at time step $$t$$.
* **$$e_t$$**: The **environment's response** (the "percept" or observation).
* **$$r_t$$**: The **reward** signal received from the environment at time $$t$$.
* **$$m$$**: The **planning horizon** (how many steps into the future the agent looks).
* **$$U$$**: The **Universal Turing Machine** (a mathematical model of a computer that simulates the environment).
* **$$q$$**: A **program** (hypothesis) running on $$U$$ that attempts to explain/predict the environment.
* **$$\text{len}(q)$$**: The **length** of the program $$q$$ in bits.
* **$$2^{-\text{len}(q)}$$**: The **prior probability** of a program. Shorter programs are considered more likely (Occam's Razor).
* **$$\arg \max_{a_t}$$**: The operator that selects the **optimal action** which results in the highest expected reward.
* **$$\sum [r_t + \dots + r_m]$$**: The **cumulative reward** the agent aims to maximize over time.

### How it Works
1. **Solomonoff Induction:** The right side of the formula calculates the probability of the environment's behavior by favoring the simplest programs ($q$) that fit the data.
2. **Expectiminimax:** The nested **max** and **sum** operators represent the agent choosing its best move while accounting for all possible environmental outcomes.
