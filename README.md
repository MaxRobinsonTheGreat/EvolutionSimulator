# EVOLUTION SIMULATOR
Designed and programmed by Max Robinson  

## What is this?
This program is designed to simulate the natural processes of evolution and population growth/decline.
It places "organisms" in an environment in which they are allowed to eat, survive, and reproduce. Over time, changes in their
anatomy accumulate and allow certain organisms to thrive while others die out. There is no goal to this system - as organisms adapt,
their competitors must adapt as well. This gives rise to many interesting and unexpected consequences. You can run it by cloning this
repo and opening the file, or by going [here](https://students.cs.byu.edu/~maximo5/EvolutionSimulation).

## Controls
- Press ```space``` to pause the simulation and see stats
- Press ```up``` arrow to speed up the simulation (boundless framerate and no visuals)
- Press ```down``` arrow to go back to normal speed with visuals

## Rules
- The organisms live on a grid.
- Each organism is composed of "cells", which occupy a single grid location
- Cells have different types, which provide certain services(see the Cell Types key below)
- Once an organism has eaten as much food as it has cells in its body, it reproduces
- Each new child has a slim chance that it may mutate, meaing it could grow, change, or lose one cell
- Once an organism has run out of time or is killed by another organism it will die
- When an organism dies, the grid is populated with food wherever the organisms' cells previously were
- The simulation runs indefinitely

## Cell Types
- GREEN - Food. This cell does NOT belong in organism anatomies. It is eaten when touched by Mouth cells 
- ORANGE - Mouth. Collects food that is directly adjacent to it.
- WHITE - Producer. Generates food in locations directly adjacent to it.
- BLUE - Mover. Allows the organisms to move randomly. It does not matter where this cell is located
- RED - Killer. Kills organisms that have cells in locations adjacent to it and turns them into food.
- PURPLE - Armor. Negates the effects of the killer cell if one touches it.

## Notes:
This program was written with very little knowledge of programming techniques or javascript. Hence, it is very
poor code quality. It was uploaded simply for preservation. However, the concept is executed with relatively good efficiency 
and, if allowed to run on its own, can produce incredible results. All ideas and code were produced by Max Robinson alone.
