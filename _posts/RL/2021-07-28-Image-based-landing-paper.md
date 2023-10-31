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
  teaser: /assets/images/Journal/ImageBased/los_alamos_video.gif
published: true
gallery:
  - url: /assets/images/Journal/ImageBased/results.png
    image_path: /assets/images/Journal/ImageBased/results.png
    alt: "placeholder image 1"
---
{% include gallery %}

<div style="text-align: justify;">
<font size="3">

Future exploration and human missions on large planetary bodies (e.g., moon, Mars) will require advanced guidance navigation and control algorithms for the powered descent phase, which must be capable of unprecedented levels of autonomy. The advent of machine learning, and specifically reinforcement learning, has enabled new
possibilities for closed-loop autonomous guidance and navigation. In this paper, image-based reinforcement meta-learning is applied to solve the lunar pinpoint powered descent and landing task with uncertain dynamic parameters and actuator failure. The agent, a deep neural network, takes real-time images and ranging observations acquired during the descent and maps them directly to thrust command (i.e., sensor-to-action policy). Training and validation of the algorithm and Monte Carlo simulations shows that the resulting closed-loop guidance policy reaches errors in the order of meters in different scenarios, even when the environment is partially observed, and the state of the spacecraft is not fully known.


Here the goal is to employ a RML approach to devise a deep network that maps, in a closed-loop fashion, sequence of images and radar altimetry data directly into trust. The latter poses a completely new challenge: since the network input is comprised by sequences of 2D images as well as ranging observations, the closed-loop NN policy become much larger in the parameter spaces. Importantly, a novel integrated environment for photo-realistic rendering which interfaces in real-time with the learning algorithm, is developed for fast training and validation. Specifically, we created a simulator that integrates dynamics and sensor data acquisition seamlessly in a python environment, that generates accurate images using lunar digital terrain models (DTM) and a physically-based rendering engine. We leverage the python-based Blender platform with dynamical models to create the powered descent and landing simulation environment accounting for both sensing and dynamics.
The proposed RML policy integrates guidance and navigation in a single compact system that is capable of mapping sequences of observations to thrust command. This is carried out in an adaptive way within the defined distribution boundaries. Specifically, some parameters of the environment, such as the gravity acceleration and the initial spacecraft mass, are randomly sampled within some distributions, which allows the meta-learner to learn over a wide distribution of instances of a stochastic environment. Moreover, random actuator failures are introduced during training, which makes the algorithm robust to such events as well. This approach allows to obtain a complete integration of guidance and navigation in a image-based closed-loop system that is robust to perturbations and un-modeled dynamics. 

<!-- {% include figure image_path="/assets/images/Journal/ImageBased/results.png" %} -->

<p><br></p>

Reference:
Scorsoglio, A., D’Ambrosio, A., Ghilardi, L., Gaudet, B., Curti, F., & Furfaro, R. (2021). Image-Based Deep Reinforcement Meta-Learning for Autonomous Lunar Landing. Journal of Spacecraft and Rockets, 1-13. <a href="https://doi.org/10.2514/1.a35072">DOI</a>

</font>
</div>
