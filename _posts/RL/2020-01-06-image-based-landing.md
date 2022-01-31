---
title: "Image-based deep reinforcement learning for autonomous lunar landing"
excerpt_separator: "<!--more-->"
categories:
  - Reinforcement Learning
tags:
  - RL
  - Relative Motion
  - Lyapunov Vector Fields
header:
  teaser: /assets/images/Conf/Orlando/image_based_conference.gif
published: true
---

Future missions to the Moon and Mars will require advanced guidance navigation and control algorithms for the powered descent phase. These algorithm should be capable of reconstructing the state of the spacecraft using the inputs from an array of sensors and apply the required command to ensure pinpoint landing accuracy, possibly in an optimal way. This has historically been solved using off-line architectures that rely on the computation of the optimal trajectory beforehand which is then used to drive the controller. The advent of machine learning and artificial intelligence has opened new possibilities for closed-loop optimal guidance. Specifically, the use of reinforcement learning can lead to intelligent systems that learn from a simulated environment how to perform optimally a certain task. In this paper we present an adaptive landing algorithm that learns from experience how to derive the optimal thrust in a lunar pinpoint landing problem using images and altimeter data as input.

We propose a new approach based on meta reinforcement learning (meta-RL) that integrates guidance and navigation functions providing a complete solution to the lunar landing problem that integrates an image-based navigation to an intelligent guidance. More specifically, we design a simulation environment that is able to integrate the dynamics of the system and simulate image acquisition from on-board cameras. This is achieved by interfacing the simulator in Python with a ray tracer (i.e. Blender) that generates accurate images using lunar digital terrain models (DTM) and a physically based rendering engine. The images are then used to update a policy in real time using reinforcement learning. We take advantage of the latest discoveries in Convolutional Neural Net (CNN) and Recurrent Neural Nets (RNN) for image processing and Proximal Policy Optimization (PPO) to design our agent and learn the optimal policy for soft landing.

{% include figure image_path="/assets/images/Conf/Orlando/Apollo16_lowCont.png" caption="DTM" %}

{% include figure image_path="/assets/images/Conf/Orlando/Apollo16_reduced.png" caption="Render" %}