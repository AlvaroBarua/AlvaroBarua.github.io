---
title: Physics Engine
date: 2018-02-01 15:49:51
category: Personal Work
thumbnail: /thumbnails/physics.jpg
---

{% youtube w6p2U3D5SIc %}

I developed this Physics Engine as part of the Advanced Game Technologies coursework.
It implements a Newtonian solver using Semi-Implicit Euler Integration and has the following elements:

- Collision shapes for both boxes and spheres.
- Distance constraints.
- Collision resolution.
- Collision event handling.
- Collision nullification to use as trigger.
- Broadphase culling (Octree and SAP).
- OpenCL accelerated manifold solver (Not completely stable, can be deactivated).

Overall, it was a challenging project, but physics programming is not exactly something I find particularly exciting.