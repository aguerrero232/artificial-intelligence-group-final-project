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



