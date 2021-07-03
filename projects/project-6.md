---
layout: project
type: project
image: images/spsp.png
title: Pathfinding Algorithms
permalink: projects/Pathfinding
# All dates must be YYYY-MM-DD format!
date: 2021-07-01
labels:
  - Algorithms
  - Visualization
  - Python
summary: An algorithm visualization and comparison for shortest path algorithms: specifically Dijkstra's and Bellman-Fords algorithms.
---

<img class="ui medium right floated rounded image" src="../images/sssp.png">

The shortest path problem in computer science is the problem of finding the shortest path between two vertices or nodes in a graph. Last semester during my Spring semester, I learned of this problem and some solutions to the problem that can solve it in a reasonable amount of time. The two algorithms I learned that solve this problem are Dijkstra's and Bellman-Ford's algorithms. [Dijkstra's algorithm](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm) takes a greedy algorithm approach and checks adjacent nodes for the shortest distance between it's neighbors, then does the same thing with the shortest distanced neighbor until the end is found, then the path is reconstructed. Although negative edges are not allowed in Dijkstra's algorithm, it runs in O(V + E log V). The [Bellman-Ford algorithm](https://en.wikipedia.org/wiki/Bellman%E2%80%93Ford_algorithm) takes a dynamic programming approach and maps the shortest path from the source to all of the vertices, then reconstructs the path to the destination node. The Bellman-Ford algorithm can detect negative cycles, and runs in O(VE).

In this project, I used [Python's Pygame library](https://www.pygame.org/) to allow users to set a source node and a destination node on the grid and compare both of the algorithms. Using pygame, users are also allowed to turn nodes into barriers on the grid, and find the path without passing through those barriers. Users are also able to edit the edge weights of nodes, reset the grid, and choose to visualize the Bellman-Ford or Dijkstra's algorithm. The program calculates one of the algorithms and visualizes it, while the other one is calculated without any visualization, and a pop up window shows a comparison between the operations needed between the two. 

In creating this project, I was able to see how much of a difference the runtime is between Bellman-Ford and Dijkstra's algorithm is, as often times when testing the program Dijkstra's algorithm ran much faster than Bellman-Fords due to the large amount of vertices and edges in the grid. I was also able to learn how pygame works, as well as learn how much faster dictionaries are than lists, since the dictionaries act as sets. Currently, the program does not notify the user of the controls, and I can improve the program by implementing that. I could also implement Dijkstra's algorithm using Fibonacci heaps instead of normal sets, and make comparisons between the two.

Source: <a href="https://github.com/PrestonTGarcia/Pathfinder"><i class="large github icon"></i>PrestonTGarcia/Pathfinder</a>
