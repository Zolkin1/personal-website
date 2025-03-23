---
title: Layered Nonlinear Model Predictive Control for Robust Stabilization of Hybrid Systems
---

## Abstract
Computing the receding horizon optimal control of nonlinear hybrid systems is typically prohibitively slow, limiting real-time implementation. To address this challenge, we propose a layered Model Predictive Control (MPC) architecture for robust stabilization of hybrid systems. A high level "hybrid" MPC is solved at a slow rate to produce a stabilizing hybrid trajectory, potentially sub-optimally, including a domain and guard sequence.  This domain and guard sequence is passed to a low level "fixed mode" MPC which is a traditional, time-varying, state-constrained MPC that can be solved rapidly, e.g., using nonlinear programming (NLP) tools. A robust version of the fixed mode MPC is constructed by using tracking error tubes that are not guaranteed to have finite size for all time. Using these tubes, we demonstrate that the speed at which the fixed mode MPC is re-calculated is directly tied to the robustness of the system, thereby justifying the layered approach. Finally, simulation examples of a five link bipedal robot and a controlled nonlinear bouncing ball are used to illustrate the formal results.

![](/research/images/layered_mpc_hybrid_fig.jpg "The hybrid MPC layer determines a feasible path at a slow rate, and passes these modes to the fixed mode MPC. This MPC computes a robustly stabilizing solution at a higher rate. The trajectory and feed forward input is passed to the low level controller where it is tracked. We use properties of the low level controller to determine the size of the tube. The resulting control action is applied to the dynamics.")

## Additional Info
**Authors**: Zachary Olkin, Aaron Ames

**Conference:** ACC 2025 (American Control Conference)

**Location of work**: Amber Lab, Caltech

**Dates of work**: May 2024 - September 2024

**Paper**: [arxiv](https://arxiv.org/abs/2503.12810v1)

[Github](https://github.com/Zolkin1/hybrid-mpc). Note that the code was not designed as a library. This is just the code to re-create the examples.