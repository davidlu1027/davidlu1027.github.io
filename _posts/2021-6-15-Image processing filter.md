---
title: Image processing filter
date: 2021-6-15 09:52:00 +0800
categories: [Circuit Design, Speech]
tags:  [accelerator]     # TAG names should always be lowercase
---

# Architecture:
![About me picture](pic/dscnn.png)

<center>DSCNN[1]</center>
 
While standard convolution performs the channelwise and spatial-wise computation in one step, Depthwise Separable Convolution splits the computation into two steps: depthwise convolution applies a single convolutional filter per each input channel and pointwise convolution is used to create a linear combination of the output of the depthwise convolution. [2]

# Design

![About me picture](pic/acc.png)

Reference

[1]Yu-Ming Tu., Tsung-Te Liu. Hardware-Efficient Keyword Spotting System(2022) 
[2]https://paperswithcode.com/method/depthwise-separable-convolution