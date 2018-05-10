---
title: AI/Networking
date: 2018-02-01 15:49:59
category: Personal Work
---

{% youtube gbbyjBGkV_8 %}

I developed this project as part of the Advanced Game Technologies coursework.
It employs both Networking and AI techniques to deliver the whole experience, some of the features are as follow.

- Random maze generation using [Prim's Algorithm.](https://en.wikipedia.org/wiki/Prim%27s_algorithm).
- Navmesh generation for the generated maze.
- [A* Algorithm](https://en.wikipedia.org/wiki/A*_search_algorithm) to calculate the path between two nodes.
- Server/Client architecture to synchronize client positions, broadcast maze structure, govern AI agents and handle physic simulation.
- Data-driven [Finite State Machine](https://en.wikipedia.org/wiki/Finite-state_machine) to handle AI behaviour.
- Client movement calculations use string pulling to minimize path nodes.
- [Dead Reckoning](https://en.wikipedia.org/wiki/Dead_reckoning) is employed to allow a smoother simulation on the client side.

This was a really fun project for me, as I am very fond of network programming, also combining our previously developed {% post_link physics %} with networking, gave me a better understanding of how some games are actually made.