---
layout: post
title: "Virtual Assistants"
author: "David Weinflash"
categories: journal
tags: [documentation,sample]
image: EpicKitchens.jpg
---

The most effective virtual assistants help users perform tasks within and beyond their skill set. Any domain specific knowledge held by the assistant is transferred to the user in the form of intuitive, timely advice. Ultimately, feedback from the assistant is both helpful and nonintrusive. 

In the following research project, I partnered with the [Four Eyes Lab at UC Santa Barbara](https://ilab.cs.ucsb.edu/) to investigate the effectiveness of baseline action recognition models in enabling nonintrusive task guidance. Through offline and real-time video analysis, we demonstrate knowledge transfer between assistant and user by way of our augmented reality application, _The AR Cooking Helper_. Using contemporary action recognition models trained on the [EPIC-KITCHENS](https://epic-kitchens.github.io/2021) dataset, we walk a user through a recipe, issuing real-time guidance when necessary to most effectively deliver perceptually-enabled task guidance.

<p style="margin-top: 10px; margin-bottom: 10px;">
  <img src="/assets/img/ARCookingHelper.png" alt="The AR Cooking Helper" style="display: block; margin: 0 auto;">
</p>

## Goals

* Explore contemporary technologies in building the ideal virtual assistant, or an assistant that is competent, perceptive and capable of providing timely advice to enhance user performance.

* Utilize a _Temporal Segment Network_ trained on the EPIC-KITCHENS dataset to assess the effectiveness of baseline action recognition models in promoting perceptually-enabled task guidance and knowledge transfer.

* Develop an augmented reality virtual assistant, or _The AR Cooking Helper_, to provide recipe instruction in the kitchen. 

  * Utilize action recognition, object recognition, textual recommendations, plane tracking and video tutorials to deliver virtual assistance.

## Takeaways

* _Temporal Segment Network_ a novel framework for video-based action recognition.

  * The framework avoids many of the common pitfalls mainstream ConvNet frameworks encounter when performing action recognition.

* _Temporal Segment Network_ performs accurately in an offline setting but poorly in a real-time setting.

  * **Offline Video Analysis** - Network performed surprisingly well when analyzing offline videos acquired from either the EPIC-KITCHENS dataset or my own home video collection.

  * **Real-Time Video Analysis** - Network performed poorly when attempting to classify actions (both cooking and cleaning) in a real-time setting.

* When paired with object recognition, action recognition and instruction step memory, augmented reality proved to be a very effective tool in facilitating knowledge transfer and task guidance.

## Documents

* [Presentation](/assets/pdf/MSProject_Presentation.pdf)
* [Report](/assets/pdf/MSProject_Report.pdf)
* [Code](https://github.com/dweinflash/ARCookingHelper)
