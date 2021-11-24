---
title: "Reinventing experience replay: prioritize like humans do"
excerpt: "A novel version of prioritized experience replay (PER) <br/><img src='/images/exp-replay.png' style='width: 500px'>"
collection: portfolio
---

This is the project I worked on with [Prof. Marcelo Mattar](https://mattarlab.ucsd.edu/). We aim to design a bias term in addition to the **TD-error** (prediction error) which was originally used in [Prioritized Experience Replay](https://arxiv.org/abs/1511.05952). This bias term, which we call the **"need" term**, measures the expected future relevance of one state w.r.t. another. The effect we want to achieve is that, given that the agent is at one certain current state, it not only samples the experiences that are most "surprising", but also most relevant to its near future.

Intuitively, if I'm preparing for a math exam, I recap those knowledge that I do not fully understand (**most surprising, high TD-error**). Meanwhile, I only recap knowledge in math (**most relevant, high need value**), instead of knowledge in physics which seems pretty irrelevant to the exam tomorrow. In this way, I get well prepared for the exam in the most efficient manner.

We thus improve PER with this bias term, calculated from **Successor Representation (SR)**. As a result, our proposed algorithm scores higher in 7 out of 10 Atari games, achieving up to **500%** improvement, as shown in the figure below, where bars with positive values indicate improvements.
<img src='/images/exp-replay.png'>
