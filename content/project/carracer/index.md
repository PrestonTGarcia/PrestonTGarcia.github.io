---
title: Car Racer
date: 2022-05-22
tags: 
    - Reinforcement Learning
    - Machine Learning
    - Computer Vision
---

An assignment finished in ICS 435 Machine Learning Fundamentals where reinforcement learning is used to train a model to play a car racing game

<!--more-->

Reinforcement learning is a method commonly used in machine learning where an machine learning model, known as an agent, is deployed into a simulation and rewards the agent for doing actions that interact with the environment correctly and penalized for interacting with the environment incorrectly. Reinforcement learning was applied in this project to train a self driving car in a small car racing game.

Each agent would be given frames of the game and would be trained to choose an action between 7 different options: do nothing, turn left and brake, turn right, turn right and brake, accelerate, or brake. Convolutional neural network, max pooling, flatten, and dense layers were all applied to the images to compress the image data down to a 7 length probability vector representing the probability to do each of the actions. Agents would be penalized by touching the grass in the car racing game, and were rewarded for staying on the road. Methods such as early stopping, hand tuning learning rate, validation sizes, and layers were applied to avoid overfitting the agents, which would result in the agents staying still instead of actually driving. 

Doing this project was my introduction to image processing and reinforcement learning. Experience in buiding neural networks was gained as prior to this I had only built machine learning models in Sklearn. The model has some flaws, as shown in the video below, some ways to improve the model could be by automating hyperparameter optimization and additional training as most of the training was constrained to one day through google colab's GPU capabilities.

Source: <a href="https://github.com/PrestonTGarcia/CarRacer"><i class="large github icon"></i>PrestonTGarcia/CarRacer</a>

Video: <a href="https://www.youtube.com/watch?v=bLgwDijX0YE"><i class="large youtube icon"></i>Preston Garcia: Car Racer</a>
