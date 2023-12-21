# Ants-Vs.-SomeBees
### 1. Introduction

a tower defense game called Ants Vs. SomeBees, inspired by a famous PopCap game--Plants Vs. Zombies. 

### 2. Files in this project:

* `ants.py`: The game logic of Ants Vs. SomeBees
* `ants_gui.py`: The original GUI for Ants Vs. SomeBees
* `graphics.py`: Utilities for displaying simple two-dimensional animations
* `utils.py`: Some functions to facilitate the game interface
* `ucb.py`: Utility functions for CS 61A
* `assets`: A directory of images and files used by `gui.py`
* `img`: A directory of images used by `ants_gui.py`

<img width="607" alt="image" src="https://github.com/ezhang114514/Ants/assets/140210568/980b057d-d66b-4c91-863c-e990b78cf3d5">

### 3. Rules:

The game of Ants vs. Bees consists of a series of rounds. In each turn, new bees may enter the ant colony. Then, new ants are assigned to defend their colony. Finally, all the insects (first the ants, then the bees) take individual actions. The bees either try to move toward the end of the tunnel or sting the ants that get in their way. The ants, in turn, take different actions depending on their type, such as gathering more food or throwing leaves at the bees. The game either ends when one bee reaches the end of the tunnel (you lose) or when the entire fleet of bees is wiped out (you win).

### 4. Playing the Game
The game can be run in two modes: as a text-based game or using a graphical user interface (GUI). The game logic is the same in either case, but the GUI enforces a turn time limit that makes playing the game more exciting. The text-based interface is provided for debugging and development.

To start a text-based game, run
```sh
$ python3 ants_text.py
````
To start a graphical game, run
```sh
$ python3 ants_gui.py
````
    usage: ants_text.py [-h] [-d DIFFICULTY] [-w] [--food FOOD]
    
    Play Ants vs. SomeBees
    
    optional arguments:
      -h, --help     show this help message and exit
      -d DIFFICULTY  sets difficulty of game (test/easy/medium/hard/extra-hard)
      -w, --water    loads a full layout with water
      --food FOOD    number of food to start with when testing
