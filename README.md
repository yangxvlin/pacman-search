# pacman
[UC Berkeley CS188 Intro to AI - Project 1](https://inst.eecs.berkeley.edu/~cs188/fa18/project1.html)

&

[unimelb COMP90054 2018 Project 1](./docs/Assignment_1.pdf)

## how to run
1. mark src as ```source root```
2. First, test that the SearchAgent is working correctly by running: 
```python pacman.py -l tinyMaze -p SearchAgent -a fn=tinyMazeSearch```
3. run ```main``` in ```autograder.py```

## my notes
1. ```problem.getSuccessors``` return: ```[(next_state from `current_state` by `aciton`, DIRECTION, step_cost)]```
2. If Pacman moves too slowly for you, try the option ```--frameTime 0```.