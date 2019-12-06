# pacman-search
[UC Berkeley CS188 Intro to AI - Project 1](https://inst.eecs.berkeley.edu/~cs188/fa18/project1.html)

&

[unimelb COMP90054 2018 Project 1](./docs/Assignment_1.pdf)

## how to run
1. mark src as ```source root```
2. First, test that the SearchAgent is working correctly by running: 
```python pacman.py -l tinyMaze -p SearchAgent -a fn=tinyMazeSearch```
3. run ```main``` in ```autograder.py```
4. run for part 1 run ```python pacman.py -l mediumMaze -p SearchAgent -a fn=ids```

    ```
    [SearchAgent] using function ids
    [SearchAgent] using problem type PositionSearchProblem
    Path found with total cost of 70 in 0.1 seconds
    Search nodes expanded: 8635
    Pacman emerges victorious! Score: 440
    Average Score: 440.0
    Scores:        440.0
    Win Rate:      1/1 (1.00)
    Record:        Win
    ```
5. run for part 2 run ```python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=wastar,heuristic=manhattanHeuristic```
    
    ```
    [SearchAgent] using function wastar and heuristic manhattanHeuristic
    [SearchAgent] using problem type PositionSearchProblem
    Path found with total cost of 210 in 0.0 seconds
    Search nodes expanded: 510
    Pacman emerges victorious! Score: 300
    Average Score: 300.0
    Scores:        300.0
    Win Rate:      1/1 (1.00)
    Record:        Win
    ```

6. run for part 3 run ```python pacman.py -l capsuleSearch -p CapsuleSearchAgent -a fn=wastar,prob=CapsuleSearchProblem,heuristic=foodHeuristic```

    ```
    [SearchAgent] using function wastar and heuristic foodHeuristic
    [SearchAgent] using problem type CapsuleSearchProblem
    Path found with total cost of 42 in 2.8 seconds
    Search nodes expanded: 1379
    Pacman emerges victorious! Score: 548
    Average Score: 548.0
    Scores:        548.0
    Win Rate:      1/1 (1.00)
    Record:        Win
    ```

    What's more, I have [```capsuleSearch2.lay```](./src/layouts/capsuleSearch2.lay). And it is made up based on [```capsuleClassic.lay ```](./src/layouts/capsuleClassic.lay)
    
    ```
    [SearchAgent] using function wastar and heuristic foodHeuristic
    [SearchAgent] using problem type CapsuleSearchProblem
    Path found with total cost of 70 in 33.7 seconds
    Search nodes expanded: 4839
    Pacman emerges victorious! Score: 670
    Average Score: 670.0
    Scores:        670.0
    Win Rate:      1/1 (1.00)
    Record:        Win
    ```

## my notes
1. ```problem.getSuccessors``` return: ```[(next_state from `current_state` by `aciton`, DIRECTION, step_cost)]```
2. If Pacman moves too slowly for you, try the option ```--frameTime 0```.