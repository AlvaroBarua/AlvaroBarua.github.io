---
title: GlitchEngine V2
date: 2018-01-10 23:20:17
category: Personal Work
---

{% youtube pUz7ZxG-uPY %}

I presented this project as part of the graphics module of the MSc I am currently undertaking.
I decided to not use the framework provided and instead work on my own idea because I wanted to make a second version of my own engine, but this time including the ability to use 3D and also have the entity component system directly on the C++ side, so I had to take this into consideration while building the framework.

This time around I used GLFW3 for window and input handling instead of SDL2 because I felt that SDL2 had too many things I would never use.

The features present in the video are as follow:
- Real-time directional shadow maps. 
- Real-time omnidirectional shadow maps. 
- Shadow accumulation. 
- All lighting calculations are done on deferred shading including shadows. 
- Text rendering using the FreeType library. 
- Bloom (Emissive extract and Blur) and Chromatic aberration post-processing effects. 
- Skinned Mesh skeletal animations. 
- Environmental mapping. Skybox and water reflections. 
- Custom model and animation loading using Assimp. 
- Tessellation shader for incrementing cylinder mesh faces and achieving laser effect. 
- Slope-based terrain texturing using the angle of the normal vector to mix 2 textures. 
- Entity Component System.
- PostProcessing stack to add or remove effects.
- Scene Graph based on the transform component of game entities.
- Frustrum culling.
- Terrain generation from a heightmap.
- Proper handling of transparent objects in deferred rendering.

Unfortunately, because of time constraints, I no longer work on this project, but in the event I find some free time, I would rewrite the framework once again, avoiding some bumps I came across the road that had ugly patches that "just work" in order to have an even cleaner and more efficient system.