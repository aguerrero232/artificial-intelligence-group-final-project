# &emsp;&emsp;&emsp; Artificial Intelligence Group Final Project

## Object Detection for Self Driving UGV Using LiDAR and RGB Data

___

## Contributors

* Daniel Brun - cur882
* Daniel Jamison - mkb622
* Ariel Guerrero - aes604
* Johann Tschetter - pzt638

___

## Objective

Transform raw data into usable point based representations. Work on data after gathering and processing it for self driving mechanisms in real time. Some parameters we must consider for the real time processing is average position, distance, and concentration of points in a certain area. When done properly, our algorithm will be able to determine the rover’s optimal path

___

## Description

The system has an Ubuntu 18.04 OS, where ROS was installed and deployed. To explain a big picture,” ROS consists of code and tools that help your project’s code run and do the required job—including the infrastructure for running it, like messages passing between processes. ROS is designed to be a loosely coupled system where a process is called a node and every node should be responsible for one task. Nodes communicate with each other using messages passing via logical channels called topics. Each node can send or get data from the other node using the publish/subscribe model”. Tawil (2017) Using ROS, the algorithm will be deployed to change the path of the rover depending on the parameters defined when reading the real-time data coming from the LiDAR as point-cloud based points to avoid obstacles.

___

## Approach: Exploration into reinforcement learning

___

* Reinforcement learning is a method of machine learning that seeks to improve the performance of a learning algorithm by using feedback from the learning algorithm.

* Implemented a Deep Q-learning algorithm to train the agent to learn to play a game to dive deeper into topics in reinforcement and deep learning.

## Single Agent

* learning about ***discrete and continuous environments*** that agents can act on
randomly selecting appropriate actions to take in a given environment.

* code example: ***single_agent.ipynb***

## Q-Learning Agent

* learning about the ***concept of Q-Learning***, which is ***a form of reinforcement learning***
that uses a Q-table to store the Q-values of the actions that the agent can take
in a given environment.

* ***Q-Learning Algorithm***
* ***Q(s<sub>t</sub>, a<sub>t</sub>) = R<sub>t+1</sub> + gamma * max(Q(s<sub>t+1</sub>))***

* s = state
* a = action
* R<sub>t+1</sub> = reward
* gamma = discount factor
* max(Q(s<sub>t+1</sub>) = max Q value ***for all possible actions*** in state s<sub>t+1</sub>

* reference: [Q-Learning algorithm](https://en.wikipedia.org/wiki/Q-learning)

* code example: ***q_agent.ipynb***

## Q-Learning Agent with Neural Network

* Using ***Q-Learning algorithm*** and a ***Sequential Model with two dense layers*** to
dive deeper in learning about the concept of deep learning.

&emsp;&emsp;![Model for Deeplearning](./img/model.png)

* code example: ***q_agent_nn.ipynb***

### **Frozen Lake** Environment

 ![](img/frozen_lake_env.png)

***[View the repository here](https://github.com/aguerrero232/deep-q-learning-agent-nn)***

___

## Approach: Applying Reinforcement Learning to simulated environment using ml-agents and unity

* ***Unity*** is a game engine that allows you to develop and test your own games, simulations, and AI agents.

* ***Unity ML-Agents*** is a library that allows you to use Unity as a platform to train and test your own agents.

* Defined a Rolling Ball Agent that acts on the environment and learns with objective of hitting the target while avoiding the obstacles (edge of the floor).

* Learns to control its own movement velocity and to avoid falling off the edge of the floor while also hitting the target.

* Final Results: ***RollerBall. Step: 500000. Time Elapsed: 3786.616 s. Mean Reward: 0.990. Std of Reward: 0.099. Final Results***

***[View Demo Here](https://play.unity.com/mg/other/webgl-builds-187355)***
