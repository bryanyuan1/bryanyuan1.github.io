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
  - GPA: 3.918/4.000
  - Honor: Magna Cum Laude

# Field of interests

- Computer Systems
- Computer Architecture
- Accelerator
- FPGA/GPU/CPU
- Physics Simulation

# Research experience

- January 2021 - July 2022: **Research Assistant**

  - **Project**: [suturing simulation](/projects/suturing-sim)
  - [UCSD Advanced Robotics and Controls Lab](https://www.ucsdarclab.com/)
  - Duties included:
    - Created a physics engine for simulating automated surgery using the position based dynamics (PBD) algorithm.
    - Implemented the key components including physics simulator, controller, and data types following best OOP practices using OpenGL and C/C++, as well as OpenMP for parallel computing.
    - On top of the simulation engine, designed a differentiable PBD constraint formula that simulates the movements of particles in the specific case of needle injection.
    - Successfully simulated the deformation of human tissue caused by injecting the needle, proving both the engine and the formula works.
    - Utilizing the gradients, implemented a deep learning controller (Python) that enabled the DaVinci robot arm to suture wounds automatically.
  - **Supervisor**: [Professor Michael Yip](https://yip.eng.ucsd.edu/)

- December 2020 - July 2022: **Research Assistant**

  - **Project**: [reinventing experience replay](/projects/exp-replay)
  - [UCSD Mattar Lab](https://mattarlab.ucsd.edu/)
  - Duties included:
    - Improved the performance of DQN, a decision-making algorithm by designing novel methods of experience replay.
    - Designed new data storage and retrieving methods for experience replay in Q-learning, inspired by a pattern in human memory replay called “gain and need”.
    - Incorporated this improvement of sampling order to the Prioritized Experience Replay (PER) algorithm.
    - Developed pytorch scripts to train the PER algorithm on multiple GPUs using Kubernetes and Docker.
    - Achieved at most 500% higher scores than humans in playing Atari games (e.g., Battlezone, Asterix).
  - **Supervisor**: [Professor Marcelo Mattar](https://mattarlab.ucsd.edu/)

- September 2020 - June 2021: **Research Assistant**
  - **Project**: 3D Bioprinter Software
  - [UCSD Chen Lab](http://schen.ucsd.edu/lab/)
  - Duties included:
    - Created a new control software for the 3D bioprinter, enabling researchers to print complex biological tissues layer by layer.
  - **Supervisor**: [Professor Shaochen Chen](http://schen.ucsd.edu/)

# Work experience

- Jan 2024 - Present: **TikTok inc.**

  - Backend Software Engineer
  - Los Angeles, CA
  - Duties included:
    - Working on the Global Monetization team to develop backend services and data pipelines for ad delivery.
    - Maintained and refactored a C++ simulation and forecasting engine, resulting in 50% latency improvement.
    - Created a new forecasting model for ads delivery results which brings down prediction error by 15%.
    - Created data jobs using Spark/Java, supporting weekly production of 60M+ ad targeting data.
    - Optimized the access pattern to the user data in memory, improving cache hit rate and reducing latency by 28%.
    - Designed and built a data collection pipeline using Kafka to support quick profiling of the simulation engine.

- July 2022 - Jan 2023: **Qualcomm**

  - Camera Software Engineer
  - San Diego, CA
  - Duties included:
    - Designed and implemented camera software and algorithms for various Automotive (car) Customers worldwide.
    - Developed multiple API pipelines in IL (Independent Layer) between application and hardware drivers using C/C++.
    - Maintained the robust operation of 10+ Qualcomm Automotive platforms that allows fast camera dev/testing.
    - Created an automatic Python test module for features across different car sensors, reducing 90% manual work.
    - Followed the full software development cycle and the automotive industry standards (ASPICE).
    - Feature owner of the dynamic sensor orientation, enabling customers to rotate video output of surrounding view sensors.

- Jun 2019 - Aug 2019: **Posse.io**
  - Software Engineer Intern
  - Encinitas, CA
  - Duties included:
    - Full-stack developer for Buztubr (now Posse.io), the world’s first digital audience monetization trade floor.
    - Developed the registration interface for users with React and HTML/CSS, enabling one-click login functionality.
    - Refactored the old, static product landing page into fully animated pages using various JavaScript modules.
    - Simplified the payment methods registration system and removed 80% redundant code with Stripe API.
    - Created a customizable data board using Facebook API, allowing influencers to view audience statistics in real-time.

# Skills

- Programming
  - Python
  - C++
  - C#
- Tools
  - tensorflow
  - pytorch
  - OpenGL
