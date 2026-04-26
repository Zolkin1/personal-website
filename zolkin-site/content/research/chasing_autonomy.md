---
title: 'Chasing Autonomy: Dynamic Retargeting and Control Guided RL for Performant and Controllable Humanoid Running'
---


## Abstract
Humanoid robots have the promise of locomoting like humans, including fast and dynamic running. Recently, reinforcement learning (RL) controllers that can mimic human motions have become popular as they can generate very dynamic behaviors, but they are often restricted to single motion play-back which hinders their deployment in long duration and autonomous locomotion. In this paper, we present a pipeline to dynamically retarget human motions through an optimization routine with hard constraints to generate improved periodic reference libraries from a single human demonstration. We then study the effect of both the reference motion and the reward structure on the reference and commanded velocity tracking, concluding that a goal-conditioned and control-guided reward which tracks dynamically optimized human data results in the best performance. We deploy the policy on hardware, demonstrating its speed and endurance by achieving running speeds of up to 3.3 m/s on a Unitree G1 robot and traversing hundreds of meters in real-world environments. Additionally, to demonstrate the controllability of the locomotion, we use the controller in a full perception and planning autonomy stack for obstacle avoidance while running outdoors.

## Figures
![](/research/images/chasing_autonomy_hero.jpg "Demonstration of the running controller working inside on a constrained treadmill and in outdoor real world environments. The running appears human-like while still achieving the commanded speed through a combination of optimized retargeted human data and control guided reward shaping.")

## Video
Coming soon.

<!-- ## Citation:
```
TBD
``` -->

## Additional Info
**Authors**: Zachary Olkin, William Compton, Ryan Bena, Aaron Ames.

**Conference:** In review.

**Location of work**: Amber Lab, Caltech

**Dates of work**: November 2025 - March 2026

**Paper**: [arxiv](https://arxiv.org/abs/2603.25902).

[RL + Deployment Code](https://github.com/Zolkin1/robot_rl), [Trajopt Code](https://github.com/Caltech-AMBER/traj_opt). The first repo hosts all the RL code and the code to deploy on the hardware. The second repo has the code for generating the trajectories.