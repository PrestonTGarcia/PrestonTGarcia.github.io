---
layout: project
type: project
image: images/carracer.png
title: Car Racer
permalink: projects/Car_Racer
# All dates must be YYYY-MM-DD format!
date: 2022-05-14
labels:
  - Artificial Intelligence
  - Machine learning
  - Computer Vision
summary: An assignment finished in ICS 435 Machine Learning Fundamentals where we use machine learning to make a car race a track on it's own.
---

<div class="ui embed" data-source="youtube" data-id="bLgwDijX0YE"></div>

Neural networks are a type of machine learning model, in which data is passed in, and that data is passed in through a network of weights, when applied creates nodes in the neural network. These weights are applied until we achieve output nodes, which is what we will be predicting in our classification problem. Convolutional neural networks (CNN) are a class of neural networks in which neural networks are applied to multidimensional data, such as an image. In this project, CNNs were used to train a model to drive a car in a small car racing game.

[Keras](https://keras.io/) was used to create, compile, and train the CNN model in this project. To create a model, I used [Conv2D](https://keras.io/api/layers/convolution_layers/convolution2d/) and [MaxPooling2D](https://keras.io/api/layers/pooling_layers/max_pooling2d/) layers and added layers hand tuning the amount of filters, kernel size, and activation function hyperparameters for the Conv2D layers, and the pool size hyperparameter for the MaxPooling2D layers. I also used two [Dense](https://keras.io/api/layers/core_layers/dense/) layers after flattening the data to convert the output to a 7 length probability vector. After I finished that, I hand tuned the overall model hyperparameters such as early stopping, reducing learning rate, and validation size. Everything in the second cell of the notebook was done by me, and anything else was provided to me, such as the simulation of the model with [OpenAI](https://openai.com/).

Doing this project I learned about how CNNs are used in image processing, and how they can be used in reinforcement learning. I also gained experience in hand tuning a neural network, as normally for the models I create I use built in methods from [Sklearn](https://scikit-learn.org/stable/index.html) such as cross-validation. This model is not perfect, as shown in the beginning of the video above, and can be improved by automating hyperparameter optimization, implementing k fold optimization, or hand tuning the hyperparameters more.

Source: <a href="https://github.com/PrestonTGarcia/CarRacer"><i class="large github icon"></i>PrestonTGarcia/CarRacer</a>
