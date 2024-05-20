---
title: Autonomous Quadrotor Trajectory Planning and Control for In-Flight Aerial Vehicle Capture
---

## Abstract
This paper develops a path planning and control architecture for an interceptor air vehicle designed to capture small target UAVs, which are assumed to be at rest or moving slowly. The proposed architecture has three main parts. First, a geometric path planner is developed to determine the trajectory for the quadrotor to travel from its initial location to the rendezvous location. The second component of the architecture is a minimal-time thrust profile generation algorithm. The algorithm represents the quadrotor’s acceleration as a B-Spline and uses the convex-hull property of the spline to transform the constraints into functions of the control points so an optimization problem can be formulated to minimize time to capture. Lastly, a low-level controller tracks the orientation and thrust commands. In this architecture, the thrust profile and geometric path are generated independently. The proposed planning and control architecture provide one key advantage over alternative optimal control approaches: by separating the thrust profile generation from the geometric path generation, the minimal time trajectory generation problem has fewer variables and constraints to calculate, thus allowing on-board calculation of the thrust profile. Results are presented demonstrating aerial capture of targets in simulation.

![](/research/images/geo_path_vectors.png "Generated trajectory. The vehichle to capture is the ellipsoid in the center, and the controlled vehicle starts on the ground below it.")

## Additional Info
**Authors**: Zachary Olkin, Jonathan Rogers

**Location**: AREAL, Georgia Tech

**Date**: May, 2020 - January 2021

[Paper](https://ieeexplore.ieee.org/document/9438242)

[Github](https://github.com/Zolkin1/quad-sim-vehicle-capture)