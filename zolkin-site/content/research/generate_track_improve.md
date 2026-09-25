---
title: 'Generate, Track, Improve: Perceptive Multi-Skill Humanoid Locomotion with RL-Fine-Tuned Motion Generators'
---

For more videos, method details, and results, see the **[project website](https://zolkin1.github.io/generate-track-improve/)**.

## Abstract
General purpose humanoids require locomotion controllers that are multi-skill, perceptive, dynamic, and robust enough to go anywhere humans can. In this work, we present a two layer locomotion architecture: (1) a perceptive flow matching motion generator plans whole body trajectories from raw depth images while a (2) perceptive tracking policy trained with control-guided RL follows these motions. Both policies are trained on a library of terrain consistent motion clips created with dynamically optimized human data which yields both accurate velocity tracking and terrain consistent references. Our central contribution is a simple yet effective off-policy RL fine tuning loop that improves the motion generator. A structured search method is used with the generator to gather data for advantage weighted regression. This off-policy loop is much more sample efficient than on-policy residual fine tuning and improves terrain consistency on unseen geometries and skill compositions. We find that successful terrain traversals increased by up to 25 percentage points and skill selection improved by up to 80 percentage points. By using raw depth images to perceive the environment no odometry or height maps are needed, and outdoor deployment is easy. With two cameras, the policy can see terrain coming from further away and adjust its velocity regardless of the commanded speed so it can traverse the terrain. A single policy pair enables a Unitree G1 humanoid to walk, run, stand, jump on and off of boxes, and traverse stairs in outdoor environments.

## Video
{{< youtube U81SjJIKUFY>}}

## Figures
![](/research/images/gti_hero_fig.jpg "Demonstration of our perceptive control policies working across multiple terrains in indoor and outdoor settings. (a) Ascending a 15 step real world staircase including transitions into and out of the stair climb. (b) Jumping onto a box, walking across it, and jumping off the box. (c) Outdoor walking locomotion including turning onto a path. (d) Running across an indoor space. (e) Descending a real world stair case.")

## Citation:
```
@article{olkin2026generate,
  title   = {Generate, Track, Improve: Perceptive Multi-Skill Humanoid
             Locomotion with RL-Fine-Tuned Motion Generators},
  author  = {Olkin, Zachary and Compton, William D. and Ames, Aaron D.},
  year    = {2026}
}
```

## Additional Info
**Authors**: Zachary Olkin, William Compton, Aaron Ames.

**Journal:** Under review.

**Location of work**: Amber Lab, Caltech

**Paper**: [pdf](https://zolkin1.github.io/generate-track-improve/paper/generate-track-improve.pdf)

**Project website**: [zolkin1.github.io/generate-track-improve](https://zolkin1.github.io/generate-track-improve/)
