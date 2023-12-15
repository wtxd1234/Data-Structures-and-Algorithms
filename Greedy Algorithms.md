[HOME](README.md)

# Overview
Greedy algorithms are a class of algorithmic strategies that make the best possible choice at each step, with the hope of finding the global optimum. They are used in optimization problems where the goal is to find the best solution out of a set of possible solutions.

## Characteristics
- **Local Optima**: Greedy algorithms choose the best option at the current time without any consideration for future consequences.
- **Irrevocable**: Once a choice is made, it cannot be undone.
- **Simple and Intuitive**: Often straightforward to implement.
- **Efficiency**: Typically run faster because they only need to process the current step and not look at the whole problem.

## Dijkstra's Algorithm

### Purpose
- To find the shortest paths from a single source vertex to all other vertices in a weighted graph.

### Process
- Initializes distances of all vertices as infinite and distance of the source as zero, then it finds the vertex with the minimum distance from the set of vertices not yet processed.
- Updates the distances of neighboring vertices of the chosen vertex.
- Repeats the process until all vertices have been processed.

### Properties
- Does not work with graphs with negative weight edges.
- Complexity is O(V^2), but with a min-priority queue, it can be reduced to O(V + E log V), where V is the number of vertices and E is the number of edges.

## Prim's Algorithm

### Purpose
- To find the minimum spanning tree for a connected weighted graph (a tree that spans all vertices and has the minimum total edge weight).

### Process
- Starts with a single vertex and grows the spanning tree one edge at a time.
- At each step, it adds the cheapest possible connection from the tree to another vertex.

### Properties
- Like Dijkstra's, Prim's algorithm can also benefit from a priority queue and has the same time complexity when implemented with a binary heap or Fibonacci heap.
- It handles graphs with negative weights, as long as they are connected and undirected.

## Kruskal's Algorithm

### Purpose
- Another algorithm to find a minimum spanning tree for a connected weighted graph.

### Process
- Sorts all the edges from low weight to high and takes the edge with the least weight that doesn’t form a cycle, adding it to the growing forest of trees.

### Properties
- It can be implemented with disjoint-set data structures (union-find).
- Time complexity is O(E log E) or O(E log V) for sorting edges, which is generally the bottleneck.

## Applications
- Network Design: Least cost wire routing, network routing protocols.
- Scheduling Problems: Job scheduling, scheduling to minimize lateness.
- System Resource Allocation: Load balancing, distributed database query optimization.

## Conclusion
Greedy algorithms are excellent for problems where local optimization at each step leads to an overall optimal solution. They are generally simpler and more efficient than other approaches, like dynamic programming or backtracking, but they do not always provide the optimal solution for every problem. Dijkstra's, Prim's, and Kruskal's algorithms are classic examples that show how greedy strategies can be applied to network and graph problems to find efficient solutions. Understanding when and how to apply greedy algorithms is a critical skill in computer science and optimization fields.
