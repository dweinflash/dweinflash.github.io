---
layout: post
title: "Deep Learning at the Edge"
author: "David Weinflash"
categories: journal
tags: [documentation,sample]
image: Cozmo_architecture.png
---

This project integrates an [Internet of Things (IoT) device](https://www.digitaldreamlabs.com/pages/meet-cozmo), 
an [Edge Device](https://www.raspberrypi.org/) and a 
[Cloud computing environment](https://colab.research.google.com/notebooks/intro.ipynb#recent=true) 
to explore machine learning at the Edge. Specifically, the project introduces a system that uses a robot’s camera feed and a deep 
learning model trained in a Cloud environment to perform object classification on a Raspberry Pi. After setting up the infrastructure, 
the project focuses on evaluating the most optimal deep learning models to deploy at the Edge, analyzing the trade-offs between model size, 
speed and accuracy to best perform object classification.

## Goals

* Perform on-device machine learning inference on a Raspberry Pi.

* Minimize latency and optimize the computing resources between an IoT device and a deep learning framework.

* Discover an optimal image classification model for the Edge, taking into account model size, accuracy and speed.

* Train an image classification model to recognize the hand gestures "rock, paper, scissors".

## Takeaways

* Deploying machine learning models to the Edge and performing inference on-device very achievable with [TensorFlow Lite](https://www.tensorflow.org/lite).
  
* Google's EfficientNets are more effective than popular convolutional neural networks (MobileNet, ResNet, Inception-v3) at the Edge.
    * EfficientNets very compact and use _compound scaling_ to achieve high accuracy while minimizing floating point operations.

* More work is necessary to increase the model’s "rock, paper, scissors" generalizability.
    * Nonetheless, EfficientNet models provide a promising solution to delivering machine learning at the Edge.
