---
title: "Adaptive generalized ZEM-ZEV feedback guidance for planetary landing via a deep reinforcement learning approach"
excerpt_separator: "<!--more-->"
categories:
  - Reinforcement Learning
tags:
  - RL
  - Planetary Landing
  - ZEM/ZEV
header:
  teaser: /assets/images/Journal/Adaptive/trials.png
published: true
gallery:
  - url: /assets/images/Journal/Adaptive/trajectory.png
    image_path: /assets/images/Journal/Adaptive/trajectory.png
    alt: "placeholder image 1"
  - url: /assets/images/Journal/Adaptive/trajectory_3D.png
    image_path: /assets/images/Journal/Adaptive/trajectory_3D.png
    alt: "placeholder image 2"
---
{% include gallery %}

<!-- {% include figure image_path="/assets/images/Journal/Adaptive/trajectory.png" caption="2D trajectory" %} -->

Precision landing on large and small planetary bodies is a technology of utmost importance for future human and robotic exploration of the solar system. In this context, the Zero-Effort-Miss/Zero-Effort-Velocity (ZEM/ZEV) feedback guidance algorithm has been studied extensively and is still a field of active research. The algorithm, although powerful in terms of accuracy and ease of implementation, has some limitations. Therefore with this paper we present an adaptive guidance algorithm based on classical ZEM/ZEV in which machine learning is used to overcome its limitations and create a closed loop guidance algorithm that is sufficiently lightweight to be implemented on board spacecraft and flexible enough to be able to adapt to the given constraint scenario. The adopted methodology is an actor-critic reinforcement learning algorithm that learns the parameters of the above-mentioned guidance architecture according to the given problem constraints.

We propose a ZEM/ZEV-based guidance algorithm for powered descent landing that can adaptively change both guidance gains and time-to-go to generate a class of closed-loop trajectories that 1) are quasi-optimal (w.r.t. the fuel-efficiency) and 2) satisfy flight constraints (e.g. thrust constraints, glide slope). The proposed algorithm exploit recent advancements in deep reinforcement learning (e.g. deterministic policy gradient), and machine learning (e.g. Extreme Learning Machines, ELM).  
The overall structure of the guidance algorithm is unchanged with respect to the classical ZEM/ZEV, but the optimal guidance gains are determined at each time step as function of the state via a parametrized learned policy. This is achieved using a deep reinforcement learning method based on an actor-critic algorithm that learns the optimal policy parameters minimizing a specific cost function. The policy is stochastic, but only its mean, expressed as a linear combination of radial basis functions, is updated by stochastic gradient descent. The variance of the policy is kept constant and is used to ensure exploration of the state space. The critic is an Extreme Learning Machine (ELM) that approximates the value function. The approximated value function is then used by the actor to update the policy. The power of the method resides in its capability, if an adequate cost function is introduced, of satisfying virtually any constraint and in its model-free nature that, given an accurate enough dynamics simulator for the generation of sample trajectories, allows learning of the guidance law in any environment, regardless of its properties. This greatly expands the capabilities of classical ZEM/ZEV guidance, allowing for its use in a wide variety of environment and constraint combinations, giving results that are generally close to the constrained fuel optimal off-line solution. Additionally, because the guidance structure is left virtually unchanged, we are able to ensure that the adaptive algorithm is maintained globally stable regardeless of the gain adaptation.

<!-- {% include figure image_path="/assets/images/Journal/Adaptive/trajectory_3D.png" caption="3D trajectory" %}  -->

Furfaro, R., Scorsoglio, A., Linares, R., & Massari, M. (2020). Adaptive generalized ZEM-ZEV feedback guidance for planetary landing via a deep reinforcement learning approach. Acta Astronautica, 171, 156-171. [DOI](http://dx.doi.org/10.1016/j.actaastro.2020.02.051)