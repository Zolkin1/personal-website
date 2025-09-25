---
title: 'Chasing Stability: Humanoid Running via Control Lyapunov Function Guided Reinforcement Learning'
---


## Abstract
Achieving highly dynamic behaviors on humanoid robots, such as running, requires controllers that are both robust and precise, and hence difficult to design. Classical control methods offer valuable insight into how such systems can stabilize themselves, but synthesizing real-time controllers for nonlinear and hybrid dynamics remains challenging. Recently, reinforcement learning (RL) has gained popularity for locomotion control due to its ability to handle these complex dynamics. In this work, we embed ideas from nonlinear control theory, specifically control Lyapunov functions (CLFs), along with optimized dynamic reference trajectories into the reinforcement learning training process to shape the reward. This approach, CLF-RL, eliminates the need to handcraft and tune heuristic reward terms, while simultaneously encouraging certifiable stability and providing meaningful intermediate rewards to guide learning. By grounding policy learning in dynamically feasible trajectories, we expand the robot’s dynamic capabilities and enable running that includes both flight and single support phases. The resulting policy operates reliably on a treadmill and in outdoor environments, demonstrating robustness to disturbances applied to the torso and feet. Moreover, it achieves accurate global reference tracking utilizing only on-board sensors, making a critical step toward integrating these dynamic motions into a full autonomy stack.

## Video
{{< youtube zCtDQuZAomI>}}

## Figures
![](/research/images/clf_rl_running_hero_fig.jpg "Overview of our approach. Trajectory optimization through each of the hybrid domains generates desired trajectories, which are used to construct a CLF-based reward. An RL policy is trained in simulation with this reward and deployed on a real humanoid robot.")



<!-- ## Citation:
```
TBD
``` -->

## Additional Info
**Authors**: Zachary Olkin, Kejun Li, William Compton, Aaron Ames.

**Conference:** Submitted to ICRA 2026

**Location of work**: Amber Lab, Caltech

**Dates of work**: August 2025 - September 2025

**Paper**: [arxiv](https://arxiv.org/abs/2509.19573).

[RL + Deployment Code](https://github.com/Zolkin1/robot_rl), [Trajopt Code](https://github.com/Caltech-AMBER/traj_opt). The first repo hosts all the RL code and the code to deploy on the hardware. The second repo has the code for generating the trajectories.