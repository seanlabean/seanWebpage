---
layout: post
title: Deep Learning from First Principles
date: 2022-05-11 00:00:00
description: Galaxy identification using ML/DL fundamentals
---

### The Goal
We will build a novel pipeline for galaxy identification using machine learning methods.
We will create a deep learning neural network from first principles with modular hidden features, allowing for rapid experimentation and optimization of image recognition techniques.

#### Week 2 05.15.22
Decided to stick with python3 for now. More efficient ot learn the basics in a language I know rather than trying to learn a new-ish language at the same time. Will be using `numpy` and perhaps some image loading packages but that's it for now.

Questions:

1. How do convolutional neural networks work? How are they implemented in a NN, similarly to a regression/recursion layer?
- At their core, CNNs are similar to RNNs in that there is a forward propogation of weighted information going between neurons that are activated by a nonlinear activation function like a ReLU. In a RNN picture classifier, an image's data for each pixel is passed to each neuron of the next hidden layer. This results in a ton of weight parameters to calculate and update, and also loses track of spatial data. In an image, an individual pixel does not typically mean very much. But a collection of neighboring pixels may reveal more: the edge of a building, an eye, a wheel, a nose. This is where CNNs excel. As the name suggests, CNNs convolve an image's data with a filter that in some way coagulates localized pixels into a single data point (we'll talk about types of filters later). The result that is passed to the next layer is smaller (due to the convolution's reduction of neighboring pixels to a single data point) and is taking into account structural data in the image. 

2. Where can I find labled data sets of galaxy pictures?
- Not sure yet! But there has to be something out there. If anything, we can start with more classic labeled sets like written numbers or cats.

#### Week 1 05.11.22
Questions:

1. Re-solidify goals. Are we building from scratch or utilizing machine learning libraries like PyTorch or TensorFlow?
- No. We will be building from scratch using Julia.
2. What data set can we easily access and use?
- SDSS
3. What is the viability of modular hidden layers?
- Unknown. See [textbook by Michael Nielsen](http://neuralnetworksanddeeplearning.com/chap1.html) for DL review: 

### The Data
There's a few large datasets available to extract galaxy image data from. Most famously there's the [Sloan Digital Sky Survey (SDSS)](https://www.sdss.org/), the [Legacy Survey of Space and Time (LSST)](https://www.lsst.org/), as well as many other smaller surveys like the Spanish J-PAS and miniJ-PAS.

#### SDSS
SDSS is a 3 dimensional color map of 3 million+ astronomical objects from 1/3 of the sky. This data is open source and has been the backbone of countless published papers. There are a few recent publications whose methods are also open source, revealing how they go about downloading and preprocessing SDSS data.

-- Smith et al (2022)
The following are open sourced methods of Smith et al. (2022): "Realistic galaxy image simulation via score-based generative models"
[Papers with code](https://paperswithcode.com/paper/realistic-galaxy-image-simulation-via-score)

[Data download](https://github.com/Smith42/astroddpm/tree/master/data/sdss)
