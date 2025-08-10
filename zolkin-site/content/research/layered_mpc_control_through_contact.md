---
title: Locomotion on Constrained Footholds via Layered Architectures and Model Predictive Control
---

<!-- {{< callout type="info">}}

Code:
  [Hardware/Sim interface](https://github.com/Zolkin1/sample-contact-walking), [MPC Library](https://github.com/Zolkin1/torc)

Paper (PDF): TBD

Paper (Arxiv): TBD
{{< /callout >}} -->
<!-- {{< callout icon="github" >}}
  Hugo can be used to create a wide variety of websites, including blogs, portfolios, documentation sites, and more.
{{< /callout >}} -->


## Abstract
Computing stabilizing and optimal control actions for legged locomotion in real time is difficult due to the nonlinear, hybrid, and high dimensional nature of these robots. The hybrid nature of the system introduces a combination of discrete and continuous variables which causes issues for numerical optimal control. To address these challenges, we propose a layered architecture that separates the choice of discrete variables and a smooth Model Predictive Controller (MPC). The layered formulation allows for online flexibility and optimality without sacrificing real-time performance through a combination of gradient-free and gradient-based methods. The architecture leverages a sampling-based method for determining discrete variables, and a classical smooth MPC formulation using these fixed discrete variables. We demonstrate the results on a quadrupedal robot stepping over gaps and onto terrain with varying heights. In simulation, we demonstrate the controller on a humanoid robot for gap traversal. The layered approach is shown to be more optimal and reliable than common heuristic-based approaches and faster to compute than pure sampling methods.

## Video
{{< youtube pTIWqsFODQk>}}

## Pictures
![](/research/images/humanoids_layered_mpc_hero_fig_v2.jpg "Demonstration of the layered controller dynamically navigating over complex terrain and locomoting effectively on flat ground. The controller is both versatile in the terrain and actions it can stabilize and fast enough for real-time control.")



<!-- ## Citation:
```
TBD
``` -->

## Additional Info
**Authors**: Zachary Olkin, Aaron Ames

**Conference:** Humanoids 2025

**Location of work**: Amber Lab, Caltech

**Dates of work**: September 2024 - April 2025

**Paper**: [arxiv](https://arxiv.org/abs/2506.09979)

[Github repo 1](https://github.com/Zolkin1/sample-contact-walking), [Github repo 2](https://github.com/Zolkin1/torc). The second repo (TORC) has the MPC code as a library and the first repo is the code that actually runs the simulation and hardware.