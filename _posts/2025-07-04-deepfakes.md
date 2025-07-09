---
layout: post
title: "Deepfakes"
author: "David Weinflash"
categories: journal
tags: [documentation,sample]
image: Deepfakes.png
---

Just as advances in machine learning gave rise to [deepfake videos](https://en.wikipedia.org/wiki/Deepfake), so too can modern machine 
learning models be put to use to reliably detect fake media content. In this project I set out to do just that – first using deep neural networks
to generate deepfake videos, then using neural networks to correctly distinguish between fake and unaltered media content. In each scenario, I
test the system on a range of different videos in order to evaluate the effectiveness of the proposed network.

<img src="/assets/img/Deepfake.gif" alt="Deepfake Videos">

## Goals

* Utilize a generative deep neural network to create deepfake videos.

* Train a neural network architecture to accurately identify deepfake videos.

* Input a variety of altered media content to measure the effectiveness of the proposed systems.

## Takeaways

* The framework proposed in [First Order Motion Model for Image Animation](https://arxiv.org/abs/2003.00196) generates convincing deepfake videos.

* The network proposed in [Video Face Manipulation Detection Through Ensemble of CNNs](https://arxiv.org/abs/2004.07676) consistently identifies fake media content.

* Certain data augmentation operations are able to influence the classification results of the deepfake detection system.

## Documents

* [Presentation](/assets/pdf/Deepfake_Presentation.pdf)
* [Report](/assets/pdf/Deepfake_Report.pdf)
* [Code](https://github.com/dweinflash/Deepfakes)
