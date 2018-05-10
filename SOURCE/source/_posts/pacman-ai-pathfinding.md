---
title: Pacman AI and Pathfinding
date: 2018-01-10 22:45:11
category: Personal Work
---

{% youtube --o9bD-Wfmg %}

This project was made for the course of advanced algorithms during my bachelor's degree.
It implemented a simple finite state machine for the ghosts behaviour and [Johnson's  algorithm](https://en.wikipedia.org/wiki/Johnson%27s_algorithm) for pathfinding. 

The path from every node in the scene is precalculated and stored in a text file which gets loaded at runtime in order to minimize the impact on performance when a ghost needs to calculate the best path to get to its destination.