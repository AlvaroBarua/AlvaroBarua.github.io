---
title: GlitchEngine V1
date: 2018-01-09 18:26:50
category: Personal Work
thumbnail: /thumbnails/glitchengine-v1.jpg
---

This was my first attempt at putting together everything I knew about C++ and OpenGL.
It is a complete game engine that uses Lua as a scripting language, it focuses on 2D games as I was trying to make a 2D game with it.

While working on the game, I went back and forth between engine and game to fix some issues and ended ditching the game completely and working solely on the engine.

I found out that my passion lies more on the engine side of the game development process, rather than on gameplay, which I still enjoy a great deal.

## Evolution
The following short videos showcase the evolution of the engine.

- Chess

{% youtube nEIkLZCczoA %}

This was the first demo I ever built, it was only capable of handling static sprites, font rendering (using the FreeType library), saving game state to file and used an OOP approach to programming. It used the [SDL2](https://www.libsdl.org/index.php) library only to handle windows and input.


- Knights

{% youtube xTbwIiMY0XE %}

This was the second demo I built, this time around I added audio support using [OpenAL](https://www.openal.org/) (Only WAV and OGG audio files are supported), wrote rudimentary physics for the knights directly in Lua and added sprite animations.


- Kings Walk

{% youtube y6wGKZ1Sxbg %}

I built this demo for a course during my Bachelor's degree. 
This time around I added a lot of features which I list here: 
-- Proper physics by adding the [Box2D](http://box2d.org/) library.
-- Video playback support by using the [WebM + vpx](https://www.webmproject.org/code/) libraries.
-- Tilemap support ([Tiled](http://www.mapeditor.org/)).
-- Native sprite class with animation support ([Shoebox](https://renderhjs.net/shoebox/) + custom export format).
-- Asynchronous asset loading.
-- Built-in FSM with transition events (mainly for controlling animation, but not limited to it).
-- Animation events.
-- Entity Component System built on top of Lua.
-- JSON file parser.
-- Instanced rendering of objects sharing materials.
-- PostProcessing support.

- Little Shooter

{% youtube twAqI2iTb7Q %}

I built this demo for a talk I gave during an event held by my university called UPCTalks. ([Video](https://www.facebook.com/GeneracionUPC/videos/1264236927007858/)).
The aim of the talk was to attract possible students by giving them facts and data about the games industry, and a small demo of how a game evolves through the development process.