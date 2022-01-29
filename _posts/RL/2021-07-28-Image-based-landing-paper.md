---
title: "Image-Based Deep Reinforcement Meta-Learning for Autonomous Lunar Landing"
excerpt_separator: "<!--more-->"
categories:
  - Meta-Reinforcement Learning
tags:
  - RL
  - Landing
  - Computer Vision
header:
  teaser: /assets/images/los_alamos_video.gif
published: true
---


Future exploration and human missions on large planetary bodies (e.g., moon, Mars) will require advanced guidance navigation and control algorithms for the powered descent phase, which must be capable of unprecedented levels of autonomy. The advent of machine learning, and specifically reinforcement learning, has enabled new
possibilities for closed-loop autonomous guidance and navigation. In this paper, image-based reinforcement meta-learning is applied to solve the lunar pinpoint powered descent and landing task with uncertain dynamic parameters and actuator failure. The agent, a deep neural network, takes real-time images and ranging observations acquired during the descent and maps them directly to thrust command (i.e., sensor-to-action policy). Training and validation of the algorithm and Monte Carlo simulations shows that the resulting closed-loop guidance policy reaches errors in the order of meters in different scenarios, even when the environment is partially observed, and the state of the spacecraft is not fully known


