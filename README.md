# pacman
UC Berkeley CS188 Intro to AI - Project 1

## how to run
1. mark src as ```source root```
2. First, test that the SearchAgent is working correctly by running: 
```python pacman.py -l tinyMaze -p SearchAgent -a fn=tinyMazeSearch```
3. run ```main``` in ```autograder.py```

## my notes
1. ```problem.getSuccessors``` return: ```[((x, y), DIRECTION, cost)]```
2. If Pacman moves too slowly for you, try the option --frameTime 0.