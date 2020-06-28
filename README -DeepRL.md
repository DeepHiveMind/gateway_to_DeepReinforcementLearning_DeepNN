# Deep Reinforcement Learning Self evolving systems


<p> Welcome to <b> The World of Deep Reinforcement Learning- Powering Self Evolving System</b>. ***It can solve the most challenging AI problems. Today, the state of the art results are obtained by an AI that is based on Deep Reinforcement Learning***. 

In recent years, the world has witnessed an acceleration of innovations in Deep Reinforcement learning (DeepRL).Such as -
[Google’s AutoML](https://cloud.google.com/automl) is also powered by *DeepRL*. | [Beating the champion of the game Go with AlphaGo](https://deepmind.com/research/case-studies/alphago-the-story-so-far) in Y'2016 |  [OpenAI and the PPO (Proximal Policy Optimization)](https://openai.com/blog/openai-baselines-ppo/) in Y'2017 |  The resurgence of [curiosity-driven learning agents](https://eng.uber.com/go-explore/) in Y'2018 with **UberAI GoExplore** and **OpenAI RND** | Recently,  [OpenAI Five](https://openai.com/projects/five/) that beats the best Dota players in the world Y'2016-Y'2019.

As more and more companies leverage DeepRL and discover new and powerful applications, they’re calling on data scientist & AI Engineers like us to create the next wave of disruptive application/solution offerings. 

Combining the powerful principles of both deep learning and reinforcement learning, DeepRL is changing the face of many industries, including:
Medicine: to determine optimal treatments for health conditions and drug therapies.| 	Robotics: to improve robotic manipulation with minimal human supervision. | 	Industrial Automation: to integrate intelligence into complex and dynamic systems. | 	Finance: increase profitability in trading. |  	

 Let us take advantage of the global AI shift! Let us unleash the power of DRL!

	
***	
This Repo primarily includes

- **[Introduction to Industry Implementation of DeepRL](#Introduction-to-Industry-Implementation-of-Deep-RL)**
- **[Introduction to High level constructs of DeepRL](#Introduction-to-DeepRL)**
```
Agent
Environment
Action
State
Reward
Policy
Value function
Function approximator
Markov decision process (MDP)
Dynamic programming (DP)
Monte Carlo methods
Temporal Difference (TD) algorithms
Model

```
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
```
Keras-RL (Developed by Matthias Plappert- Employed with OpenAI)
OpenAI Gym
Facebook Horizon
Google Dopamine
Google DeepMind TensorFlow Reinforcement Learning (TRFL)
Coach (Developed by Intel Nervana Systems)
RLLib (Highly customizable open source DeepRL framework with support for TF2.0/PyTorch 1.4, customization for Environments/Policy/Action)
Tensorforce (Tensorforce is built on top of Google's TensorFlow framework version 2.0 by Alexander Kuhnle - currently with BluePrism)
```
- **[DeepRL HANDS-ON with Keras-RL & TF & OpenAI-Gym](#DeepRL-HANDS-ON-with-Keras-RL-GYM)**
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
- **[Interesting DeepRL framework RLlib](#Interesting-DeepRL-framework-RLlib)**
- **[DeepRL HANDS-ON Additional](#DeepRL-HANDS-ON-additional)**
- Also a reference to series of blog posts and videos 🆕 about Deep Reinforcement Learning. 

***

## Introduction to Industry Implementation of Deep RL

Deep RL is one of the key factor powering -
- Medicine: to determine optimal treatments for health conditions and drug therapies.
- Robotics: to improve robotic manipulation with minimal human supervision. 
- Finance: increase profitability in trading. 
- Industrial Automation: to integrate intelligence into complex and dynamic systems. 
- Self Evolving Control System
- Hyperautomation
- Google AutoML (NAS + Deep RL)
- TRAX ([AI with Speed in Sequence Model](https://github.com/google/trax) )
- Autocorrection, autocompletion in Email/Typing/NLP (heady mix of dynamic programming, hidden Markov models, and word embeddings) 
-  Autonomous Systems
-  Smart Deep Gaming
-  Many more

<img src="https://github.com/Deep-Mind-Hive/coach/blob/master/img/fetch_slide.gif" alt="Fetch Slide" width = "300" height ="200"/>

<img src="https://github.com/Deep-Mind-Hive/coach/blob/master/img/carla.gif" width = "300" height ="200" alt="Starcraft"/>

## Introduction to DeepRL

#### Overview
The main solution blocks of RL/DeepRL are 
- the agent and 
- the environment. 
	
  - The environment is the world that the agent lives in and interacts with. 
  - At every step of interaction, the agent sees a (possibly partial) observation of the state of the world, and then decides on an action to take. 
  - The environment changes when the agent acts on it, but may also change on its own.
  - The agent also perceives a reward signal from the environment, a number that tells it how good or bad the current world state is. 
  - The goal of the agent is to maximize its cumulative reward, called return. Reinforcement learning methods are ways that the agent can learn behaviors to achieve its goal.


#### High Level Solution Constructs of DeepRL

- High Level Solution Constructs of Deep Reinforcement Learning through Infographics

<img src="https://github.com/DeepHiveMind/gateway_to_DeepReinforcementLearning_DeepNN/blob/master/Infographics/RLDesign.png" alt="Deep Reinforcement Learning High Level Solution Constructs" width = "900" height ="400" />


- Agent — the learner and the decision maker.
- Environment — where the agent learns and decides what actions to perform.
- Action — a set of actions which the agent can perform.
- State — the state of the agent in the environment.
- Reward — for each action selected by the agent the environment provides a reward. Usually a scalar value.
- Policy — the decision-making function (control strategy) of the agent, which represents a mapping from situations to actions.
- Value function — mapping from states to real numbers, where the value of a state represents the long-term reward achieved starting from that state, and executing a particular policy.
- Function approximator — refers to the problem of inducing a function from training examples. Standard approximators include decision trees, neural networks, and nearest-neighbor methods
- Markov decision process (MDP) — A probabilistic model of a sequential decision problem, where states can be perceived exactly, and the current state and action selected determine a probability distribution on future states. Essentially, the outcome of applying an action to a state depends only on the current action and state (and not on preceding actions or states).
- Dynamic programming (DP) — is a class of solution methods for solving sequential decision problems with a compositional cost structure. Richard Bellman was one of the principal founders of this approach.
- Monte Carlo methods — A class of methods for learning of value functions, which estimates the value of a state by running many trials starting at that state, then averages the total rewards received on those trials.
- Temporal Difference (TD) algorithms — A class of learning methods, based on the idea of comparing temporally successive predictions. Possibly the single most fundamental idea in all of reinforcement learning.
- Model — The agent’s view of the environment, which maps state-action pairs to probability distributions over states. Note that not every reinforcement learning agent uses a model of its environment



Please refer to the 📜:[ARTICLE](https://medium.freecodecamp.org/an-introduction-to-reinforcement-learning-4339519de419) for further detailing into the basic constructs of DeepRL ecosystem. <br>

## Significant Deep RL Models

Deep RL Algorithms overview by Infographics
***useful taxonomy of algorithms in modern RL**

<img src="https://github.com/Deep-Mind-Hive/coach/blob/master/docs_raw/source/_static/img/algorithms.png" width = "900" height ="400" alt="Algorithms"/>

###### Value Optimization Agents Algorithms
* [Deep Q Network (DQN)](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf)  
* [Double Deep Q Network (DDQN)](https://arxiv.org/pdf/1509.06461.pdf) 
* [Dueling Q Network](https://arxiv.org/abs/1511.06581)
* [Mixed Monte Carlo (MMC)](https://arxiv.org/abs/1703.01310)
* [Persistent Advantage Learning (PAL)](https://arxiv.org/abs/1512.04860) 
* [Categorical Deep Q Network (C51)](https://arxiv.org/abs/1707.06887) 

###### Policy Optimization Agents Algorithms
* [Policy Gradients (PG)](http://www-anw.cs.umass.edu/~barto/courses/cs687/williams92simple.pdf) | *Multi Worker Single Node*  
* [Asynchronous Advantage Actor-Critic (A3C)](https://arxiv.org/abs/1602.01783) | *Multi Worker Single Node*
* [Deep Deterministic Policy Gradients (DDPG)](https://arxiv.org/abs/1509.02971) | *Multi Worker Single Node* 
* [Proximal Policy Optimization (PPO)](https://arxiv.org/pdf/1707.06347.pdf)

###### General Agents Algorithms
* [Direct Future Prediction (DFP)](https://arxiv.org/abs/1611.01779) | *Multi Worker Single Node* 


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
Keras-RL (Developed by Matthias Plappert- Employed with OpenAI)
OpenAI Gym
Facebook Horizon
Google Dopamine
Google DeepMind TensorFlow Reinforcement Learning (TRFL)
Coach (Developed by Intel Nervana Systems)
RLLib (Highly customizable open source DeepRL framework with support for TF2.0/PyTorch 1.4, customization for Environments/Policy/Action)
Tensorforce (Tensorforce is built on top of Google's TensorFlow framework version 2.0 by Alexander Kuhnle - currently with BluePrism)

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

Refer to the 📜 **[ARTICLE](https://winderresearch.com/a-comparison-of-reinforcement-learning-frameworks-dopamine-rllib-keras-rl-coach-trfl-tensorforce-coach-and-more/)** for the comparison-of-Reinforcement-learning-frameworks, such as 
	Dopamine / rllib / Keras-rl / coach /	trfl /	tensorforce /	coach

## Introduction to DeepRL Models supported by Keras RL framework

Refer to the [Repo](https://github.com/keras-rl/keras-rl) for how to implement important following Agent Models using KERAS-RL, such as

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


## Interesting DeepRL framework RLlib

Refer to [RLib frameowrk](https://docs.ray.io/en/master/rllib.html) for its USPs (Customization feature).

RLlib provides ways to *customize* almost all aspects of 
	- training, 
	- including the environment, 
	- neural network model, 
	- action distribution, and 
	- policy definitions

The following infographics shows the customization flexibility offered by RLlib - 
<br>
<img src="https://docs.ray.io/en/master/_images/rllib-components.svg" alt="Fetch Slide" width ="600" height ="400"/>

The above diagram also provides a conceptual overview of data flow between different components in RLlib -
	- We start with an *Environment*, which given an *action* produces an observation. -->
	- Then, The observation is preprocessed by a *Preprocessor* and *Filter* (e.g. for running mean normalization) before being sent to a *neural network Model* (agent Model with Policy). -->
	- The model output is in turn interpreted by an *ActionDistribution* to determine the next action.

RLlib supports both the major DeepNN frameworks for *neural network Model* (agent Model with Policy) -
- TensorFlow 2.0
- PyTorch 1.4.0

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
