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

### q2
#### test1
```python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs --frameTime 0```
```
[SearchAgent] using function bfs
[SearchAgent] using problem type PositionSearchProblem
Path found with total cost of 68 in 0.0 seconds
Search nodes expanded: 275
Pacman emerges victorious! Score: 442
Average Score: 442.0
Scores:        442.0
Win Rate:      1/1 (1.00)
Record:        Win
```

#### test2
```python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5  --frameTime 0```
```
[SearchAgent] using function bfs
[SearchAgent] using problem type PositionSearchProblem
Path found with total cost of 210 in 0.0 seconds
Search nodes expanded: 620
Pacman emerges victorious! Score: 300
Average Score: 300.0
Scores:        300.0
Win Rate:      1/1 (1.00)
Record:        Win
```

#### test3
```python eightpuzzle.py -fn=bfs```
```
D:\python\python.exe E:/backup/code/python/pacman/src/eightpuzzle.py -fn=bfs
A random puzzle:
-------------
| 3 | 5 | 1 |
-------------
| 6 | 4 |   |
-------------
| 7 | 8 | 2 |
-------------
BFS found a path of 11 moves: ['down', 'left', 'left', 'up', 'right', 'up', 'right', 'down', 'left', 'left', 'up']
After 1 move: down
-------------
| 3 | 5 | 1 |
-------------
| 6 | 4 | 2 |
-------------
| 7 | 8 |   |
-------------
Press return for the next state...

...
...
...

After 11 moves: up
-------------
|   | 1 | 2 |
-------------
| 3 | 4 | 5 |
-------------
| 6 | 7 | 8 |
-------------
Press return for the next state...
```

## my notes
1. ```problem.getSuccessors``` return: ```[((x, y), DIRECTION, cost)]```
2. If Pacman moves too slowly for you, try the option --frameTime 0.