---
title: Team Project
date: 2018-05-10 18:13:05
category: Personal Work
thumbnail: /thumbnails/team-project.jpg
---

{% youtube _bJ-0FHgj6E %}
 
{% youtube aq-7KydZTSo %}
 
{% youtube w_4A4lM9Ak4 %}
 
{% youtube 670dR90OQoE %}

This project was developed as part of the "Engineering Gaming Solutions within a Team" course, the goal of the project was to have a Splatoon-like game where you painted the environment to earn points. Our project was developed from the beginning with cross-platform development in mind and as such, we put a CMake build system in place that allowed us to change target platforms with ease, at the moment of handling the project, our game was able to run on Window/Mac/Linux/Android and PS4 with networked multiplayer among all of them.

The whole engine was developed from scratch in the span of 6 weeks by a 7 people team.

My main contributions to this projects where:
- Full rendering pipeline (OpenGL and PS4)
- Vertex painting for the paint effect using OpenCL, and GNM Compute Shaders on PS4.
- Entity Component System as the base for the engine.
- Memory usage and allocations tracking.

## Technology Used
- C++
- OpenGL
- GLSL
- GNM (PS4)
- OpenCL
- GNM Compute Shaders

## Libraries Used
- SDL2 (Window and Input handling)
- Bullet (Physics)
- GLM (Math)
- OpenALSoft (Audio, not on PS4 as we used the PS4 native audio libraries)
- ENet (Networking, we had to make a fork of the library and some changes to it, so it would also work on PS4)