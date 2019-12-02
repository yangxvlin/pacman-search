# pacman
UC Berkeley CS188 Intro to AI - Project 1

## how to run
1. mark src as ```source root```
2. First, test that the SearchAgent is working correctly by running: 
```python pacman.py -l tinyMaze -p SearchAgent -a fn=tinyMazeSearch```

### q1
```python pacman.py -l tinyMaze -p SearchAgent```  
```python pacman.py -l mediumMaze -p SearchAgent```  
```python pacman.py -l bigMaze -z .5 -p SearchAgent```

## my notes
```problem.getSuccessors``` return: ```[((x, y), DIRECTION, cost)]```