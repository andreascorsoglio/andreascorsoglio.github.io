---
title: "VisualEnv: visual Gym environments with Blender"
excerpt_separator: "<!--more-->"
categories:
  - Computer Vision
tags:
  - Computer vision
header:
  teaser: /assets/images/Journal/VisualEnv/Vcart_ext.jpg
published: false
---


VisualEnv is a tool designed for creating visual environment for reinforcement learning. It is the product of an integration of an open-source modelling and rendering software, Blender, and a python module used to generate environment models for simulation, OpenAI Gym. VisualEnv allows the user to create custom environments with photorealistic rendering capabilities and full integration with python. The framework is described and tested on a series of example problems that showcase its features for training reinforcement learning agents.

<p float="center">
  <img src="/assets/images/Journal/VisualEnv/test_Vcart.gif" width="220" />
  <img src="/assets/images/Journal/VisualEnv/test_Hover2D.gif" width="220" /> 
  <img src="/assets/images/Journal/VisualEnv/test_Goal.gif" width="220" />
</p>

The tool is built around two open-source pieces of software: Blender and OpenAI Gym. Blender is a modelling, animation and rendering software that is usually used for production quality computer graphics workflows. It offers a wide range of tools for modelling, sculpting, shading, texturing, lighting and rendering. Moreover, it interfaces easily with python through an API. OpenAI Gym on the other hand is a powerful environment builder written in python and widely used to train RL agents. VisualEnv harnesses the power of both to create a standalone package that can be used to generate custom visual environment in python. These can then be used to train RL algorithm or perform other types of real time simulation tasks. The user has control over every aspect of the rendering and animation of the environment. The environment and the actor can be created using a pletora of photorealistic shaders and materials. The environment dynamics can be controlled by the gym environment that then interfaces with blender through the API, moving and modifying the actors in the scene. The rendered observations can then be used for a variety of applications. The power of the frameworks resides in the ease of implementation and capabilities suitable for online-applications.



