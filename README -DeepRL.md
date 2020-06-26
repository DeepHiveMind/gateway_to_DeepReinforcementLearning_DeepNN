# Deep Reinforcement Learning Self evolving systems


<p> Welcome to <b> The World of Deep Reinforcement Learning- Powering Self Evolving System</b>. This Repo primarily includes

- **[Introduction to Industry Implementation of DeepRL](#Introduction-to-Industry-Implementation-of-Deep-RL)**
- **[Introduction to High level constructs of DeepRL](#Introduction-to-DeepRL)**
- **[Introduction to Significant DeepRL algorithms](#Significant-Deep-RL-Models)**
```
-Value Optimization Agents Algorithms
    -Deep Q Network (DQN)
    -Double Deep Q Network (DDQN)
    -Mixed Monte Carlo (MMC)
    
-Policy Optimization Agents Algorithms
    -Policy Gradients (PG)
    -Asynchronous Advantage Actor-Critic (A3C)
    -Deep Deterministic Policy Gradients (DDPG)
    -Proximal Policy Optimization (PPO)
 
-General Agents Algorithms
    -Direct Future Prediction (DFP)
```
- **[Introduction to Advanced DeepRL algorithms](#Advanced-Deep-RL-Models)**
```
- Imitation Learning Agents Algorithms
    -Behavioral Cloning (BC)  
    -Conditional Imitation Learning
- Hierarchical Reinforcement Learning Agents Algorithms
    -Hierarchical Actor Critic (HAC)
- Memory Types Algorithms
    -Hindsight Experience Replay (HER)
    -Prioritized Experience Replay (PER)
```
- **[Comparison of Main DeepRL frameworks](#Comparison-of-Main-DeepRL-frameworks)**
- **[DeepRL HANDS-ON with Keras-RL & TF & OpenAI-Gym](#DeepRL-HANDS-ON-with-Keras-RL-GYM)**
- **[DeepRL HANDS-ON Additional](#DeepRL-HANDS-ON-additional)**
- Also a reference to series of blog posts and videos 🆕 about Deep Reinforcement Learning. 


## Introduction to Industry Implementation of Deep RL

Deep RL is one of the key factor powering -
-  Self Evolving Control System
-  Hyperautomation
-  Google AutoML (NAS + Deep RL)
-  TRAX ([AI with Speed in Sequence Model](https://github.com/google/trax) )
-  Autocorrection, autocompletion in Email/Typing/NLP (heady mix of dynamic programming, hidden Markov models, and word embeddings) 
-  Autonomous Systems
-  Smart Deep Gaming
-  Many more

<img src="https://github.com/Deep-Mind-Hive/coach/blob/master/img/fetch_slide.gif" alt="Fetch Slide"width = "300" height ="200"/> 
<img src="https://github.com/Deep-Mind-Hive/coach/blob/master/img/carla.gif" width = "300" height ="200" alt="Starcraft"/>

## Introduction to DeepRL

- High Level Solution Constructs of Deep Reinforcement Learning through Infographics

<img src="https://github.com/DeepHiveMind/gateway_to_DeepReinforcementLearning_DeepNN/blob/master/Infographics/RLDesign.png" alt="Deep Reinforcement Learning High Level Solution Constructs" style="width: 500px;"/>

Please refer to the 📜:[ARTICLE](https://medium.freecodecamp.org/an-introduction-to-reinforcement-learning-4339519de419) <br><br>

## Significant Deep RL Models

- Deep RL Algorithms overview by Infographics

<img src="https://github.com/Deep-Mind-Hive/coach/blob/master/docs_raw/source/_static/img/algorithms.png" width = "600" height ="500" alt="Algorithms"/>

###### Value Optimization Agents Algorithms
* [Deep Q Network (DQN)](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf)  
* [Double Deep Q Network (DDQN)](https://arxiv.org/pdf/1509.06461.pdf) 
* [Dueling Q Network](https://arxiv.org/abs/1511.06581)
* [Mixed Monte Carlo (MMC)](https://arxiv.org/abs/1703.01310)
* [Persistent Advantage Learning (PAL)](https://arxiv.org/abs/1512.04860) 
* [Categorical Deep Q Network (C51)](https://arxiv.org/abs/1707.06887) 

###### Policy Optimization Agents Algorithms
* [Policy Gradients (PG)](http://www-anw.cs.umass.edu/~barto/courses/cs687/williams92simple.pdf) | **Multi Worker Single Node**  
* [Asynchronous Advantage Actor-Critic (A3C)](https://arxiv.org/abs/1602.01783) | **Multi Worker Single Node**  
* [Deep Deterministic Policy Gradients (DDPG)](https://arxiv.org/abs/1509.02971) | **Multi Worker Single Node**  
* [Proximal Policy Optimization (PPO)](https://arxiv.org/pdf/1707.06347.pdf)

###### General Agents Algorithms
* [Direct Future Prediction (DFP)](https://arxiv.org/abs/1611.01779) | **Multi Worker Single Node** 


## Advanced DeepRL Models

###### Imitation Learning Agents Algorithms
* Behavioral Cloning (BC)  
* [Conditional Imitation Learning](https://arxiv.org/abs/1710.02410)

###### Hierarchical Reinforcement Learning Agents Algorithms
* [Hierarchical Actor Critic (HAC)](https://arxiv.org/abs/1712.00948.pdf)

###### Memory Types Algorithms
* [Hindsight Experience Replay (HER)](https://arxiv.org/abs/1707.01495.pdf)
* [Prioritized Experience Replay (PER)](https://arxiv.org/abs/1511.05952) 

### Exploration Techniques Algorithms
* E-Greedy 
* Boltzmann
* Normal Noise
* Truncated Normal Noise 
* [Bootstrapped Deep Q Network](https://arxiv.org/abs/1602.04621) 


## Comparison of most common DeepRL frameworks
 
- Here are the list of Most commonly used DeepRL framework  
```
Keras-RL
Tensorforce
Facebook Horizon
OpenAI Gym
Google Dopamine
Nervana Systems Coach
RLLib
TRFL

```

- A few other DeepRL Frameworks (not so popular)
```
MAgent
SLM-Lab
DeeR
Garage
Surreal
RLgraph
Simple RL
```

- Comparison of Most commonly used Deep RL frameworks

📜 **[ARTICLE](https://winderresearch.com/a-comparison-of-reinforcement-learning-frameworks-dopamine-rllib-keras-rl-coach-trfl-tensorforce-coach-and-more/)** for the comparison-of-Reinforcement-learning-frameworks, such as 

## Introduction to DeepRL Models supported by Keras RL framework

📜 **[ARTICLE](https://github.com/keras-rl/keras-rl)** for how to implement important following Agent Models using KERAS-RL, such as

```
 Deep Q Learning (DQN)
 Double DQN 
 Deep Deterministic Policy Gradient (DDPG) 
 Continuous DQN (CDQN or NAF)
 Cross-Entropy Method (CEM)
 Dueling network DQN (Dueling DQN)
 Deep SARSA
 Asynchronous Advantage Actor-Critic (A3C)
 Proximal Policy Optimization Algorithms (PPO)
```

## DeepRL HANDS ON with Keras RL GYM

- keras-rl implements some state-of-the art deep reinforcement learning algorithms in Python and seamlessly integrates with the deep learning library Keras.
- Furthermore, keras-rl works with OpenAI Gym out of the box. This means that evaluating and playing around with different algorithms is easy.
- keras-rl can be extended according to our own custom needs. One can use built-in Keras callbacks and metrics or define one's own.

Please refer to [https://github.com/Deep-Mind-Hive/keras-rl/tree/master/examples](https://github.com/Deep-Mind-Hive/keras-rl/tree/master/examples) repo for DeepRL Agents with following algorithmic implementations - 

      - CEM_cartpole.py
      - DDPG_mujoco.py
      - DDPG_pendulum.py
      - DQN_atari.py
      - DQN_cartpole.py
      - DUEL_DQN_cartpole.py
      - NAF_pendulum.py
      - SARSA_cartpole.py
      
Please refer to repo [DeepRL HANDS-ON with Keras & TF & OpenAI-Gym](https://github.com/DeepHiveMind/keras-io/blob/master/examples/README_Keras_TF2.0_Applications_Codeset.md#deep-reinforcement-learning-hands-on-with-keras-rl--tf--openai-gym) for following DeepRL model implementations:
			
			     -Actor Critic Method
			     -Deep Deterministic Policy Gradient (DDPG)
			     -Deep Q-Learning for Atari Breakout

## DeepRL HANDS ON additional

###### Q-learning with FrozenLake

- 📜 [ARTICLE](https://medium.freecodecamp.org/diving-deeper-into-reinforcement-learning-with-q-learning-c18d0db58efe) // [FROZENLAKE IMPLEMENTATION](https://github.com/DeepHiveMind/Deep_reinforcement_learning_Course/blob/master/Q%20learning/FrozenLake/Q%20Learning%20with%20FrozenLake.ipynb)<br>

- 📹 [Implementing a Q-learning agent that plays Taxi-v2 🚕](https://youtu.be/q2ZOEFAaaI0) <br><br>

###### Deep Q-learning with Doom 
-📜 [ARTICLE](https://medium.freecodecamp.org/an-introduction-to-deep-q-learning-lets-play-doom-54d02d8017d8)  //  [DOOM IMPLEMENTATION](https://github.com/DeepHiveMind/Deep_reinforcement_learning_Course/blob/master/Deep%20Q%20Learning/Doom/Deep%20Q%20learning%20with%20Doom.ipynb)<br>

-📹 [Create a DQN Agent that learns to play Atari Space Invaders 👾](https://youtu.be/gCJyVX98KJ4) <br><br>

###### Policy Gradients with Doom
- 📜 [ARTICLE](https://medium.freecodecamp.org/an-introduction-to-policy-gradients-with-cartpole-and-doom-495b5ef2207f) //  [CARTPOLE IMPLEMENTATION](https://github.com/DeepHiveMind/Deep_reinforcement_learning_Course/blob/master/Policy%20Gradients/Cartpole/Cartpole%20REINFORCE%20Monte%20Carlo%20Policy%20Gradients.ipynb) // [DOOM IMPLEMENTATION](https://github.com/DeepHiveMind/Deep_reinforcement_learning_Course/blob/master/Policy%20Gradients/Doom/Doom%20REINFORCE%20Monte%20Carlo%20Policy%20gradients.ipynb) <br>

- 📹 [Create an Agent that learns to play Doom deathmatch](https://www.youtube.com/watch?v=wLTQRuizVyE) <br><br>

###### Improvments in Deep Q-Learning
-📜 [ARTICLE](https://medium.freecodecamp.org/improvements-in-deep-q-learning-dueling-double-dqn-prioritized-experience-replay-and-fixed-58b130cc5682)//  [Doom Deadly corridor IMPLEMENTATION](https://github.com/DeepHiveMind/Deep_reinforcement_learning_Course/blob/master/Dueling%20Double%20DQN%20with%20PER%20and%20fixed-q%20targets/Dueling%20Deep%20Q%20Learning%20with%20Doom%20(%2B%20double%20DQNs%20and%20Prioritized%20Experience%20Replay).ipynb) <br>

- 📹 [Create an Agent that learns to play Doom Deadly corridor](https://youtu.be/-Ynjw0Vl3i4) <br><br>

###### Advantage Advantage Actor Critic (A2C)
- 📜 [ARTICLE](https://medium.freecodecamp.org/an-intro-to-advantage-actor-critic-methods-lets-play-sonic-the-hedgehog-86d6240171d) <br>

- 📹 [Create an Agent that learns to play Sonic](https://youtu.be/GCfUdkCL7FQ) <br><br>

###### Proximal Policy Gradients <br>
- 📜 [ARTICLE](https://towardsdatascience.com/proximal-policy-optimization-ppo-with-sonic-the-hedgehog-2-and-3-c9c21dbed5e)<br>

- 👨‍💻 [Create an Agent that learns to play Sonic the Hedgehog 2 and 3 ](https://github.com/DeepHiveMind/Deep_reinforcement_learning_Course/tree/master/PPO%20with%20Sonic%20the%20Hedgehog) <br><br>

###### Curiosity Driven Learning made easy 
- 📜 [ARTICLE](https://towardsdatascience.com/curiosity-driven-learning-made-easy-part-i-d3e5a2263359)
