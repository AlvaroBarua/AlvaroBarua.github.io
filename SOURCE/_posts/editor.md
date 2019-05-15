---
title: T5 Editor
date: 2018-05-15 14:13:24
category: Personal Work
thumbnail: /thumbnails/t5-editor.jpg
---

After completing our team project, everyone was left with a feeling that it could become something bigger, and so, we decided to keep working on whatever we thought was a good idea for the engine. From my end, I was really unhappy with the way we managed the creation of the levels, so the obvious next step was to create a level editor.

I started by adding a library called cereal to be able to serialize classes to JSON files, after some tinkering, I was able to save the whole entity list into a single file while taking into account hierarchy, to that I added some simple things like screen clear color and current skybox; and with that I had successfully generated a simple but complete level file.

I used Qt as GUI library because it has an OpenGLWidget class that you can use to easily run OpenGL code inside a window interface, within no time, I was able to run the engine, and from there I just kept adding things, like the entity explorer (which shows all the components added to the selected entity) and the level entities list (which shows all entities with their complete scene graph hierarcy).

I also kept working on the rendering pipeline and changed the frustum culling from sphere based to AABB based, expanded the support of the GLTF format (only meshes and materials so far) and added full PBR support with the metallic roughness model.

This is a short video of the current state of the editor:
{% youtube 0fhMOhMj3ls %}

## Plans for the future
I'm planning on adding some more support for the editor itself as right now you can only position elements on the scene, I also want to implement shadow cascading and forward+ rendering as they are things I have never tried before and seem to be really fun and challenging to do.

## Update
I added CSM shadows to the engine, the video quality is not good at all because of LinkedIn compression and I lost the source video to reupload.
<br><div class="video-container"><iframe src="https://www.linkedin.com/embed/feed/update/urn:li:ugcPost:6404104557768568832?compact=1" frameborder="0" allowfullscreen></iframe></div>
