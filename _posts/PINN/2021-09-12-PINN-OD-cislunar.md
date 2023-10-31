---
title: "Orbit determination via physics informed neural networks in cislunar environment"
excerpt_separator: "<!--more-->"
categories:
  - Physics Informed Neural Networks
tags:
  - PINN
header:
  teaser: /assets/images/Conf/BigSky/halo.jpg
published: true
gallery:
  - url: /assets/images/Conf/BigSky/halo.jpg
    image_path: /assets/images/Conf/BigSky/halo.jpg
    alt: "placeholder image 1"
---
{% include gallery caption="Estimated trajectories" %}

<div style="text-align: justify;">
<font size="3"> 

The approach presented in this paper is based on using Physics Informed Neural Networks (PINN) to estimate the state of a spacecraft in cislunar space given angles measurements. The novel concept introduced by PINNs is the ability to solve forward and inverse problems governed by parametric Differential Equations (DEs). This is done by approximating the solution of the DE using a neural network which is trained by embedding the dynamical model into the NN loss function. This acts as a regularizer that penalizes the network's training when the physics of the problem is violated. PINN have been successfully used in a variety of works, spanning from computational gas dynamics to spacecraft guidance and control. When used to solve the OD problem, PINN allows the solution to be physically sound and, in the meantime, avoids the need for proper initialization. The method presented can use angle measurements (e.g., right ascension, declination) and the knowledge of the dynamical system to create an accurate estimation of the state of the system. This is particularly useful for objects moving in cislunar space where the CRTBP framework governs the dynamics. Moreover, this method can estimate the entire trajectory without needing propagation steps that are computationally expensive and prone to errors.</div>


Reference:
Scorsoglio, A., Ghilardi, L., & Furfaro, R. (2023). A Physic-Informed Neural Network Approach to Orbit Determination. The Journal of the Astronautical Sciences, 70(4), 1-30. <a href="https://doi.org/10.1007/s40295-023-00392-w">DOI</a>

</font>
</div>

<!-- {% include figure image_path="/assets/images/Conf/BigSky/halo.jpg" alt="" caption="Estimated trajectory for halo orbit" %} -->