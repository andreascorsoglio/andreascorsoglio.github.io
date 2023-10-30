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
  teaser: /assets/images/Conf/LakeTahoe/lake_tahoe_real.gif
published: true
gallery:
  - url: /assets/images/Conf/LakeTahoe/lake_tahoe_real.gif
    image_path: /assets/images/Conf/LakeTahoe/lake_tahoe_real.gif
    alt: "placeholder image 1"
  - url: /assets/images/Conf/LakeTahoe/lake_tahoe_mask.gif
    image_path: /assets/images/Conf/LakeTahoe/lake_tahoe_mask.gif
    alt: "placeholder image 2"
  - url: /assets/images/Conf/LakeTahoe/lake_tahoe_hazard.gif
    image_path: /assets/images/Conf/LakeTahoe/lake_tahoe_hazard.gif
    alt: "placeholder image 3"
---

{% include gallery caption="Ground view, segmentation mask and hazard map." %}

<font size="3">

<div style="text-align: justify;">
In this paper, we propose a new approach based on deep learning that integrates guidance and navigation functions, providing a complete solution to the lunar landing problem that integrates image-based navigation to intelligent guidance. We exploit the latest advancements in computer vision and Convolutional Neural Network (CNN) to implement a hazard detection and avoidance algorithm to detect safe landing sites autonomously. As it can be noted, the approach we propose is entirely based on machine learning algorithms (semantic segmentation), whereas the procedure used for the Chang'e-3 mission was still based on optical images, but the detection was performed via more "classical" edge detection algorithms. The CNN for hazard detection and avoidance is trained in a supervised fashion and is then embedded in the guidance framework. In order to do this, we designed a simulation environment that is able to integrate the dynamics of the system and simulate image acquisition from onboard cameras. This is achieved by interfacing the simulator in Python with a ray tracer (i.e., Blender) that generates accurate images using lunar Digital Terrain Models (DTM) and a physically-based rendering engine. The control policy is trained to align the boresight direction of the ground-facing camera to a target on the ground using reinforcement learning, specifically an actor-critic algorithm called Proximal Policy Optimization (PPO). The hazard detection and avoidance subroutine is then used at the testing phase to assign a safe area on the ground as a target for the policy in order to perform a targeted soft landing.</div>

<!-- {% include figure image_path="/assets/images/Conf/LakeTahoe/lake_tahoe_real.gif" caption="Ground View" %}

{% include figure image_path="/assets/images/Conf/LakeTahoe/lake_tahoe_mask.gif" caption="Ground Mask" %}

{% include figure image_path="/assets/images/Conf/LakeTahoe/lake_tahoe_hazard.gif" caption="Ground Hazard map" %} -->
<p><br></p>

Reference:
Scorsoglio, A., D’Ambrosio, A., Ghilardi, L., Furfaro, R., Gaudet, B., Linares, R., & Curti, F. (2020, August). Safe Lunar landing via images: A Reinforcement Meta-Learning application to autonomous hazard avoidance and landing. In Proceedings of the 2020 AAS/AIAA Astrodynamics Specialist Conference, Virtual (pp. 9-12). [DOI](https://www.researchgate.net/profile/Andrea-Scorsoglio/publication/343650361_Safe_lunar_landing_via_images_a_reinforcement_meta-learning_application_to_autonomous_hazard_avoidance_and_landing/links/60b94f15a6fdcc22ead3c19b/Safe-lunar-landing-via-images-a-reinforcement-meta-learning-application-to-autonomous-hazard-avoidance-and-landing.pdf)