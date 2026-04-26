---
title: 'Stability of Control Lyapunov Function Guided Reinforcement Learning'
---


## Abstract
Reinforcement learning (RL) has become the de facto method for achieving locomotion on humanoid robots in practice, yet stability analysis of the corresponding control policies is lacking. Recent work has attempted to merge control theoretic ideas with reinforcement learning through control guided learning. A notable example of this is the use of a control Lyapunov function (CLF) to synthesize the reinforcement learning rewards, a technique known as CLF-RL, which has shown practical success. This paper investigates the stability properties of optimal controllers using CLF-RL with the goal of bridging experimentally observed stability with theoretical guarantees. The RL problem is viewed as an optimal control problem and exponential stability is proven in both continuous and discrete time using both core CLF reward terms and the additional terms used in practice. The theoretical bounds are numerically verified on systems such as the double integrator and cart-pole. Finally, the CLF guided rewards are implemented for a walking humanoid robot to generate stable periodic orbits.

## Figures
![](/research/images/clf_rl_theory_hero.jpg "The main ideas behind CLF guided RL. A CLF is designed offline and used in an RL/optimal control problem as the reward/cost. Then the optimal policy is applied to the system resulting in provable exponential stability and in stable humanoid locomotion.")

<!-- ## Citation:
```
TBD
``` -->

## Additional Info
**Authors**: Zachary Olkin, William Compton, Aaron Ames.

**Conference:** In review.

**Location of work**: Amber Lab, Caltech

**Dates of work**: Feburary 2026 - March 2026

**Paper**: Coming soon.
