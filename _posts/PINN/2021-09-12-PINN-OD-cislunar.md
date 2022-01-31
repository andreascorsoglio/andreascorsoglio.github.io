---
title: "Orbit determination via physics informed neural networks in cislunar environment"
excerpt_separator: "<!--more-->"
categories:
  - Physics Informed Neural Networks
tags:
  - PINN
header:
  teaser: /assets/images/Conf/BigSky/PIOD_nonKep.png
published: true
---

The approach presented in this paper is based on using Physics Informed Neural Networks (PINN) to estimate the state of a spacecraft in cislunar space given angles measurements. The novel concept introduced by PINNs is the ability to solve forward and inverse problems governed by parametric Differential Equations (DEs). This is done by approximating the solution of the DE using a neural network which is trained by embedding the dynamical model into the NN loss function. This acts as a regularizer that penalizes the network's training when the physics of the problem is violated. PINN have been successfully used in a variety of works, spanning from computational gas dynamics to spacecraft guidance and control. When used to solve the OD problem, PINN allows the solution to be physically sound and, in the meantime, avoids the need for proper initialization. The method presented can use angle measurements (e.g., right ascension, declination) and the knowledge of the dynamical system to create an accurate estimation of the state of the system. This is particularly useful for objects moving in cislunar space where the CRTBP framework governs the dynamics. Moreover, this method can estimate the entire trajectory without needing propagation steps that are computationally expensive and prone to errors.


{% include figure image_path="/assets/images/Conf/halo.png" alt="" caption="Estimated trajectory for halo orbit" %}