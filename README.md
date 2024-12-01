# Pacman AI Search Agent

This repository contains the implementation of various search algorithms (**DFS**, **BFS**, **UCS**) used to navigate Pacman through different mazes. The goal is to explore how different search strategies influence performance in terms of **path cost**, **nodes expanded**, and **execution time**.

The project is based on UC Berkeley's CS188 course on Artificial Intelligence. For more information about the project structure and objectives, you can refer to the [UC Berkeley AI Project Overview](https://ai.berkeley.edu/project_overview.html).

---

## Algorithms Implemented

1. **Depth-First Search (DFS)**  
   - Explores the deepest nodes in the search tree first.  
   - May not always find the shortest path but is efficient in terms of implementation.

2. **Breadth-First Search (BFS)**  
   - Explores the shallowest nodes first and guarantees the shortest path for uniform cost mazes.  

3. **Uniform Cost Search (UCS)**  
   - Expands nodes in order of least path cost and finds the optimal path for mazes with varying costs.

---

## Running the Game

To run the Pacman game with the implemented search algorithms, use the following commands. Replace `mediumMaze` with `tinyMaze`, `bigMaze`, or other layouts for different maze complexities.

### For Depth-First Search (DFS):
```bash
python pacman.py -l mediumMaze -p SearchAgent -a fn=dfs
```

### For Breadth-First Search (BFS):
```bash
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
```

### For Uniform Cost Search (UCS):
```bash
python pacman.py -l mediumMaze -p SearchAgent -a fn=ucs
```

---


## Performance Comparison of Search Algorithms

| Algorithm | Maze       | Path Cost | Nodes Expanded | Score | Win Rate  |
|-----------|------------|-----------|----------------|-------|-----------|
| DFS       | tinyMaze   | 10        | 15             | 500   | 1/1 (1.00)|
| BFS       | tinyMaze   | 8         | 15             | 502   | 1/1 (1.00)|
| UCS       | tinyMaze   | 8         | 15             | 502   | 1/1 (1.00)|
| DFS       | mediumMaze | 130       | 146            | 380   | 1/1 (1.00)|
| BFS       | mediumMaze | 68        | 269            | 442   | 1/1 (1.00)|
| UCS       | mediumMaze | 68        | 269            | 442   | 1/1 (1.00)|
| DFS       | bigMaze    | 210       | 390            | 300   | 1/1 (1.00)|
| BFS       | bigMaze    | 210       | 620            | 300   | 1/1 (1.00)|
| UCS       | bigMaze    | 210       | 620            | 300   | 1/1 (1.00)|


---

## Visual Comparisons

To make it easier to interpret the results, visualizations such as bar graphs or line charts can highlight the differences in **path cost**, **nodes expanded**, and **time taken** for each algorithm across mazes. 


## About the Project

This project demonstrates the strengths and weaknesses of fundamental AI search strategies. It serves as an educational exercise in understanding and applying algorithmic concepts to real-world challenges. The repository is modular, allowing further development and experimentation with more advanced search algorithms.

