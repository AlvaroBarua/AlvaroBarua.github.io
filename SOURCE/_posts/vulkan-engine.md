---
title: Vulkan Engine
date: 2019-05-14 20:45:03
category: Personal Work
thumbnail: /thumbnails/vulkan-engine.jpg
---

## Why?
As you can see from other posts, I have been working with OpenGL for quite some time and I feel that I am at a point in which I don't know everything about it, but feel confident enough to work with it in a professional environment. So, in order to keep up with the current trends, I decided to learn Vulkan, I am currently still learning things about it and taking it slow to make sure I learn it well as well as developing a robust engine architecture in order to support multiple graphics API's.

{% asset_img GameView.jpg %}

As of right now, the "engine" if you can call it that at this stage in development, have the following features:
- Offline shader multi-compiler using glslc.
- Technique like files that define pipeline state and shader passes for a material.
- Material system that allows enabling/disabling shader defines at runtime.
- Multi-threaded renderer.
- Entity-Component driven.
- Clear separation in systems to allow multiple API's.
- Easy to swap between different lightning models.
- GLTF (Meshses and Materials) and DDS (2D and CubeMap) formats support.

## Editor

{% asset_img EditorView.jpg Editor %}

As part of the development, and mainly because of the shader multi-compiler (I needed a way of defining material properties so that I didn't have to load a technique file with 16K+ shader permutations every time), I decided to implement an editor. 

This time around I don't want it to be just a level editor, but a complete editor with live objects editing and all the bell and whistles modern engines have. As I had already worked on Qt, this time I wanted to try something different and went with ImGui which has been surprisingly easy to use.

The editor is still in early development stages but already have the following:
- Scene Graph tree.
- Entity explorer, where all the components are shown with their expose variables.
- A log window with different categories and search filter.
- Resource explorer with directory watcher that updates in real-time.
- Scene graph drag and drop to reparent transforms.

## What's Next

There are still a lot of features I would like to add to both of them such as:

### Engine
- Indirect drawing of static objects with GPU culling using material batching.
- Cascade shadow maps using probably VSM to get better quality soft shadows.
- Terrain rendering with frustum culling, indirect drawing and tessellation.
- Depth, Normals and Motion Vectors pre-pass.
- Post-processing stack.
- Physics using PhysX.

### Editor
- Scene serialization.
- Full support for all basic engine features.
- User components reflection without the need of adding them to the editor project by generating stub components from the .h files.
- Network link between editor and game to synchronize the state of the game on the editor and be able to edit components or add objects on the fly for faster iteration.