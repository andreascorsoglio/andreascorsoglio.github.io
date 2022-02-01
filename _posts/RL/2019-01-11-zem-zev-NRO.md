---
title: "Actor-critic reinforcement learning approach to relative motion guidance in near-rectilinear orbit"
excerpt_separator: "<!--more-->"
categories:
  - Reinforcement Learning
tags:
  - RL
  - Relative Motion
  - ZEM/ZEV
header:
  teaser: /assets/images/Conf/Hawaii/L2_south.png
published: true
gallery:
  - url: /assets/images/Conf/Hawaii/trajectoryLVLH_1.png
    image_path: /assets/images/Conf/Hawaii/trajectoryLVLH_1.png
    alt: "placeholder image 1"
  - url: /assets/images/Conf/Hawaii/trajectoryLVLH_2.png
    image_path: /assets/images/Conf/Hawaii/trajectoryLVLH_2.png
    alt: "placeholder image 2"
---

{% include gallery caption="Trajectories" %}

This paper aims a developing a new feedback guidance algorithm for docking maneuvers in the cislunar environment. In particular, the goal is to create an algorithm that is lightweight, closed-loop and capable of taking path constraints into account. The problem has been solved starting from the well know Zero-Effort-Miss/Zero-Effort-Velocity (ZEM/ZEV) guidance using machine learning to improve its capabilities and widen its field of application. The algorithm has been developed in the circular restricted three body problem (CRTBP) framework for Near Rectilinear Orbits (NRO) in the Earth-Moon system but the results can be easily generalized to many more guidance problems. The results are satisfactory and show that reinforcement learning can be effectively used to solve constrained relative spacecraft guidance problems.

<!-- {% include figure image_path="/assets/images/Conf/Hawaii/trajectoryLVLH_1.png" %}

{% include figure image_path="/assets/images/Conf/Hawaii/trajectoryLVLH_2.png" %} -->

