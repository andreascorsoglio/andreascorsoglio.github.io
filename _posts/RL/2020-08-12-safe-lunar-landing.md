---
title: "Safe Lunar landing via images: A Reinforcement Meta-Learning application to autonomous hazard avoidance and landing"
excerpt_separator: "<!--more-->"
categories:
  - Reinforcement Learning
tags:
  - RL
  - Landing
  - Computer Vision
header:
  teaser: /assets/images/Conf/LakeTahoe/real.gif
published: true
---

In this paper, we propose a new approach based on deep learning that integrates guidance and navigation functions, providing a complete solution to the lunar landing problem that integrates image-based navigation to intelligent guidance. We exploit the latest advancements in computer vision and Convolutional Neural Network (CNN) to implement a hazard detection and avoidance algorithm to detect safe landing sites autonomously. As it can be noted, the approach we propose is entirely based on machine learning algorithms (semantic segmentation), whereas the procedure used for the Chang'e-3 mission was still based on optical images, but the detection was performed via more "classical" edge detection algorithms. The CNN for hazard detection and avoidance is trained in a supervised fashion and is then embedded in the guidance framework. In order to do this, we designed a simulation environment that is able to integrate the dynamics of the system and simulate image acquisition from onboard cameras. This is achieved by interfacing the simulator in Python with a ray tracer (i.e., Blender) that generates accurate images using lunar Digital Terrain Models (DTM) and a physically-based rendering engine. The control policy is trained to align the boresight direction of the ground-facing camera to a target on the ground using reinforcement learning, specifically an actor-critic algorithm called Proximal Policy Optimization (PPO). The hazard detection and avoidance subroutine is then used at the testing phase to assign a safe area on the ground as a target for the policy in order to perform a targeted soft landing.


{% include figure image_path="/assets/images/Conf/LakeTahoe/lake_tahoe_real.gif" caption="Ground View" %}

{% include figure image_path="/assets/images/Conf/LakeTahoe/lake_tahoe_mask.gif" caption="Ground Mask" %}

{% include figure image_path="/assets/images/Conf/LakeTahoe/lake_tahoe_hazard.gif" caption="Ground Hazard map" %}