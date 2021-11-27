---
title: "Suturing Simulation: a novel 3D environment"
excerpt: "A simulation environment for suturing automation<br/><img src='/images/suturingsim.gif' style='width: 500px'>"
collection: projects
---

This the project at [UCSD Advanced Robotics and Controls Lab](https://www.ucsdarclab.com/). Our goal is to automate surgical suturing using deep Reinforcement Learning methods, by training a robotic arm to hold the tissue in fixed position while the needle sutures and pushes the tissue. However, to enable training such a complex task, we need to build a simulation environment in the computer first, so the algorithms can be sufficiently trained before eventually deployed to the real robot arms. In particular, we need to simulate how the tissue deforms due to the motion of the needle. Thus, it was my responsibility to build such a simulator using OpenGL. 

This simulation environment simulates the deformation of human tissue when a needle penetrates inside. It can be shown in the picture below that the tissue is pressed down when the needle thrusts in, and it gets stretched upwards when the needle goes out. This effect is achieved by the simulation method of [position-based dynamics (PBD)](https://matthias-research.github.io/pages/publications/posBasedDyn.pdf) and a novel PBD constraint function I proposed to simulate friction force. For now, it already realistically simulates the real operation, but we are continuing to make improvements. 

Meanwhile, we are curious whether we can find the gradients of the positions using PBD. That leads to our ongoing work of **diffPBD**, a novel differentiable physics solver. We hope that not only would our simulator provide a training environment for RL, but also enables direct gradient-based control for the robotic arm to holds the tissue in the right place.

**Note**: The black dots aligned in a semi-circular shape represents a simplified model of the suturing needle.

<img src='/images/suturingsim.gif'>
