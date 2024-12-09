---
title: Bilevel Optimization for Real-Time Control with Application to Locomotion Gait Generation
---

## Abstract
Model Predictive Control (MPC) is a common tool for the control of nonlinear, real-world systems, such as legged robots. However, solving MPC quickly enough to enable its use in real-time is often challenging. One common solution is given by real-time iterations, which does not solve the MPC problem to convergence, but rather close enough to give an approximate solution. In this paper, we extend this idea to a bilevel control framework where a "high-level" optimization program modifies a controller parameter of a "low-level" MPC problem which generates the control inputs and desired state trajectory. We propose an algorithm to iterate on this bilevel program in real-time and provide conditions for its convergence and improvements in stability. We then demonstrate the efficacy of this algorithm by applying it to a quadrupedal robot where the high-level problem optimizes a contact schedule in real-time. We show through simulation that the algorithm can yield improvements in disturbance rejection and optimality, while creating qualitatively new gaits. 

![](/research/images/bilevel_gait_gen.jpg "Structure of the bilevel optimization. The MPC uses parameters from the high-level optimization and outputs the control inputs and state trajectory. When applied to the quadruped, the high-level parameter is the contact schedule. The green dots indicate contact with the ground and show how the contact schedule changes over time.")

## Additional Info
**Authors**: Zachary Olkin, Aaron Ames

**Location**: Amber Lab, Caltech

**Date**: October 2023 - April 2024

Paper: [arXiv](https://arxiv.org/abs/2409.12366)

[Github](https://github.com/Zolkin1/bilevel-gait-gen)