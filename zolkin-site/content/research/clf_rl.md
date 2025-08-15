---
title: 'CLF-RL: Control Lyapunov Function Guided Reinforcement Learning'
---


## Abstract
Reinforcement learning (RL) has shown promise in generating robust locomotion policies for bipedal robots, but often suffers from tedious reward design and sensitivity to poorly shaped objectives. In this work, we propose a structured reward shaping framework that leverages model-based trajectory generation and control Lyapunov functions (CLFs) to guide policy learning. We explore two model-based planners for generating reference trajectories: a reduced-order linear inverted pendulum (LIP) model for velocity-conditioned motion planning, and a precomputed gait library based on hybrid zero dynamics (HZD) using full-order dynamics. These planners define desired end-effector and joint trajectories, which are used to construct CLF-based rewards that penalize tracking error and encourage rapid convergence. This formulation provides meaningful intermediate rewards, and is straightforward to implement once a reference is available. Both the reference trajectories and CLF shaping are used only during training, resulting in a lightweight policy at deployment. We validate our method both in simulation and through extensive real-world experiments on a Unitree G1 robot. CLF-RL demonstrates significantly improved robustness relative to the baseline RL policy and better performance than a classic tracking reward RL formulation.

## Video
{{< youtube f8iuwgCZs3A>}}

## Figures
![](/research/images/clf_rl_hero_fig.jpg "Overview of our approach. A reference generator produces target trajectories, which are used to construct a CLF-based reward. An RL policy is trained in simulation with this reward and deployed on a real humanoid robot.")



<!-- ## Citation:
```
TBD
``` -->

## Additional Info
**Authors**: Kejun Li*, Zachary Olkin*, Yisong Yue, Aaron Ames (* indicates equal contribution).

**Journal:** Submitted to RA-L

**Location of work**: Amber Lab, Caltech

**Dates of work**: June 2025 - August 2025

**Paper**: [arxiv](https://arxiv.org/abs/2508.09354)

[RL + Deployment Code](https://github.com/Zolkin1/robot_rl), [Trajopt Code](https://github.com/Caltech-AMBER/traj_opt). The first repo hosts all the RL code and the code to deploy on the hardware. The second repo has the code for generating the trajectories.