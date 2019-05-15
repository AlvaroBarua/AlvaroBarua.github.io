---
title: Tactics AI
date: 2018-01-10 22:45:19
category: Personal Work
thumbnail: /thumbnails/tactics-ai.jpg
---

{% youtube _v-HQldMh70 %}

This project was developed for the Artificial Intelligence course during my bachelor’s degree.
It was a team project, but as I was the only one that knew how to use Unity, I was in charge of every aspect of the implementation. My teammates helped me with the graphic design and algorithm design.

For this particular case, we design a [MinMax algorithm](https://en.wikipedia.org/wiki/Minimax) that took into account position, health and defence state to calculate the optimal move. When playing on easy, the AI uses a completely random approach, in medium, the AI only calculates its move based on the current playfield, and in hard, it takes into account all the possible moves of the enemy in the next turn and makes a choice based on the score obtained for every possible choice.