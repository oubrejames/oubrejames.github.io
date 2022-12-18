---
layout: post
title:  "Physics Simulation"
categories: [ Python, Hack-a-Thon 2021, Group Project ]
image: assets/images/cropped_jack.gif
featured: true
hidden: true
---
Python / PyGame


<div align="center"><img src="https://raw.githubusercontent.com/oubrejames/oubrejames.github.io/4b9a9bb1b282e894d9406c93f0adbf26e34a60b5/assets/images/cropped_jack.gif" alt="jack_box_gif" width="500"/></div>



I worked with a team to generate and solve a maze using recursive backtracking. My teammate generated solveable mazes represented by numerical arrays, and I used PyGame to create the maze graphics of wall (black), open path (white), the start (green), and end (red) squares along with a visual indicator of which index the solver visits (blue). The solver starts at the "start" index and randomly selects an adjacent index. If the selected index has a value of 1, it is added to the wall list and a different index is chosen. If the index is open (value of 0), the algorithm "moves" to the index and chooses a new adjacent index. Any index that the algorithm finds and moves to is added to a path list, which are only allowed to be selected again if no other open index exists. Any index that leads to backtracking is added to a wall list. The blue searching square becomes cyan when it is forced to backtrack.

### [View it on Github](https://github.com/oubrejames/physics-simulator)
