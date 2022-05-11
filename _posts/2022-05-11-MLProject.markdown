---
layout: post
title: Deep Learning from First Principles
date: 2022-05-11 00:00:00
description: Galaxy identification using ML/DL fundamentals
---

# The Goal
We will build a novel pipeline for galaxy identification using machine learning methods.
We will create a deep learning neural network from first principles with modular hidden features, allowing for rapid experimentation and optimization of image recognition techniques.

## Questions (05/11/22) 
1. Re-solidify goals. Are we building from scratch or utilizing machine learning libraries like PyTorch or TensorFlow?
2. What data set can we easily access and use?
3. What is the viability of modular hidden layers?

# The Data
There's a few large datasets available to extract galaxy image data from. Most famously there's the [Sloan Digital Sky Survey (SDSS)](https://www.sdss.org/), the [Legacy Survey of Space and Time (LSST)](https://www.lsst.org/), as well as many other smaller surveys like the Spanish J-PAS and miniJ-PAS.

## SDSS
SDSS is a 3 dimensional color map of 3 million+ astronomical objects from 1/3 of the sky. This data is open source and has been the backbone of countless published papers. There are a few recent publications whose methods are also open source, revealing how they go about downloading and preprocessing SDSS data.

-- Smith et al (2022)
The following are open sourced methods of Smith et al. (2022): "Realistic galaxy image simulation via score-based generative models"
[Papers with code](https://paperswithcode.com/paper/realistic-galaxy-image-simulation-via-score)

[Data download](https://github.com/Smith42/astroddpm/tree/master/data/sdss)
