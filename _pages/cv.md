---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

# Education

- B.S. in Computer Science, University of California San Diego, 2021

# Field of interests

- Reinforcement Learning
- Surgical Robotics
- Neuroscience
- Physics Simulation

# Work experience

- January 2021 - Present: **Research Assistant**

  - **Project**: [suturing simulation](/projects/suturing-sim)
  - [UCSD Advanced Robotics and Controls Lab](https://www.ucsdarclab.com/)
  - Duties included:
    - Developed a simulation environment using OpenGL and position based dynamics (PBD) to train robots for automated surgery.
    - Successfully simulated the deformation of the tissue during suturing with a new constraint formula, appearing more real than existing solutions.
    - Derived a novel physics simulation method called diffPBD by making PBD differentiable, enabling direct gradient-based control of a gripper to deform the tissue towards the target shape.
  - **Supervisor**: [Professor Michael Yip](https://yip.eng.ucsd.edu/)

- December 2020 - Present: **Research Assistant**

  - **Project**: [reinventing experience replay](/projects/exp-replay)
  - [UCSD Mattar Lab](https://mattarlab.ucsd.edu/)
  - Duties included:
    - Used ideas from the human memory replay pattern, the need and gain terms, to design a novel experience replay method in Q-learning.
    - Monitored training tasks on Nautilus, UCSD’s kubernetes cluster, enabling learning with multiple GPUs.
    - Redesigned the sampling order in the prioritized sweeping algorithm (PS), resulting in faster convergence to the optimal policy in the Gridworld game.
    - Incorporated deep successor representation into prioritized experience replay (PER), resulting in at most a 500% performance increase in Atari games (e.g., Battlezone, Asterix).
  - **Supervisor**: [Professor Marcelo Mattar](https://mattarlab.ucsd.edu/)

- September 2020 - June 2021: **Research Assistant**
  - **Project**: 3D Bioprinter Software
  - [UCSD Chen Lab](http://schen.ucsd.edu/lab/)
  - Duties included:
    - Created a new control software for the 3D bioprinter, enabling researchers to print complex biological tissues layer by layer.
  - **Supervisor**: [Professor Shaochen Chen](http://schen.ucsd.edu/)

# Skills

- Programming
  - Python
  - C++
  - C#
- Tools
  - tensorflow
  - pytorch
  - OpenGL

# Publications

  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
