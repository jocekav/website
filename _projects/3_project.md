---
layout: page
title: FOREST
description: Developing generative music and dance for robotic arms
img: assets/img/7.jpg
redirect: https://unsplash.com
importance: 3
category: work
---

FOREST is an NSF funded project aimed at enhancing trust between humans and robots through sound and gesture. I focused on generative music and robotic dances based on patterns. The project used 10 robotic XArm factory robots controlled by Python and Matlab scripts.

# Game of Life
Cellular automata are a grids of cells with finite states. The state of a cell is modified by a simple algorithm that is influenced by the state's of neighboring cells. 'Game of Life' is the most famous cellular automaton, simulating the dynamical evolution of a society of living organisms.
I created a variation on the "Game of Life" to simulate relationships between a group of robots. I extended the algorithm to create aesthetic visual and musical patterns for performance. I extended the traditional rules of the "Game of Life" to encourage more pattern creation on 10 robots.
The 'Game' has 4 states, birth, death, living, and dying, and each of these states are mapped to a robot gesture. A robot's state is determined by its neighbor's states according to the rules below. The starting states are randomized and the 'Game' can continue for any number of iterations. Additionally, the game can start with a contagion effect with the first robot defined as alive then living.

# Flocking
After studying cellular automaton, I pursued another simulation of emergent behavior in the natural world through flocking. We want to see if we can achieve a flocking behavior with high levels of entitativity despite a limited number of units in a fixed grid.
I used a variation of the Boids algorithm. Boids algorithm is built on 3 rules: cohesion, adhesion, and separtation. Boids algorithm uses mobile agents with state changes informed by an agent's position, velocity, and acceleration. Because the xArm robots are fixed in a grid, the flocking algorithm was modified to use the angles of the robot's seven joints.