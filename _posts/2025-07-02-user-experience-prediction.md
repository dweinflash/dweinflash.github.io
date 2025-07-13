---
layout: post
title: "User Experience Prediction"
author: "David Weinflash"
categories: journal
tags: [documentation,sample]
image: QoE_Results.png
---

Quality of experience (QoE) has become an increasingly important metric for today’s modern service providers.
Discovering and optimizing the factors that determine user experience has thus become an essential goal for
network operators. In this project, I teamed with the [Mobility Management and Networking (MOMENT) Lab](https://moment.cs.ucsb.edu/) 
at UC Santa Barbara to focus on exploring the link between key radio measurements and user experience in the context of video streaming sessions.

## Goals

* Explore several machine learning algorithms to predict quality of experience from radio and network measurements.

  * Random Forest
  * ARIMA 
  * Recurrent Neural Network (LSTM)

* Investigate the effect of radio measurements and quality of service (QoS) metrics on quality of experience.

  * **Radio Measurement**: Reference Signal Received Power (RSRP)
  * **Quality of Service Measurement**: Throughput

## Takeaways

* Random Forest and ARIMA can be used to predict buffer level with high accuracy, precision and recall.

  * Random forest model was especially effective in segmenting network level measurements using both a quantile binning and uniform binning approach.
    
  * ARIMA able to quickly output accurate predictions on QoE using a linear regression model based on lagged observations.
  
* Simpler models perform noticeably better than compute-intensive LSTM networks.

## Documents

* [Presentation](/assets/pdf/QoE_Presentation.pdf)
* [Report](/assets/pdf/QoE_Report.pdf)
* [Code](https://github.com/dweinflash/NetworkingAI)
