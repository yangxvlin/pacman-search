# pacman
UC Berkeley CS188 Intro to AI - Project 1

## how to run
1. mark src as ```source root```
2. First, test that the SearchAgent is working correctly by running: 
```python pacman.py -l tinyMaze -p SearchAgent -a fn=tinyMazeSearch```

### q1
#### test1
```python pacman.py -l tinyMaze -p SearchAgent```  
```
[SearchAgent] using function depthFirstSearch
[SearchAgent] using problem type PositionSearchProblem
Path found with total cost of 10 in 0.0 seconds
Search nodes expanded: 15
Pacman emerges victorious! Score: 500
Average Score: 500.0
Scores:        500.0
Win Rate:      1/1 (1.00)
Record:        Win
```

#### test2
```python pacman.py -l mediumMaze -p SearchAgent```  
```
[SearchAgent] using function depthFirstSearch
[SearchAgent] using problem type PositionSearchProblem
Path found with total cost of 130 in 0.0 seconds
Search nodes expanded: 146
Pacman emerges victorious! Score: 380
Average Score: 380.0
Scores:        380.0
Win Rate:      1/1 (1.00)
Record:        Win
```

#### test3
```python pacman.py -l bigMaze -z .5 -p SearchAgent```
```
[SearchAgent] using function depthFirstSearch
[SearchAgent] using problem type PositionSearchProblem
Path found with total cost of 210 in 0.0 seconds
Search nodes expanded: 390
Pacman emerges victorious! Score: 300
Average Score: 300.0
Scores:        300.0
Win Rate:      1/1 (1.00)
Record:        Win
```

## my notes
```problem.getSuccessors``` return: ```[((x, y), DIRECTION, cost)]```