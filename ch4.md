The General Shortest-Path Problem
=================================

Introduction
------------

* Shortest path in a general directed graph.

Acyclic Networks
----------------

* Graphs with no cycle.

* Topologic order: DP stages.

* Can find not only shortest distance but also longest one.

General Networks
----------------

* No natural ordering.

* Dijkstra algorithm: path length as DP order/stages.

* Bellman-Ford: `k` iterations determine the shortest path when `k` or fewer arcs must be used.

* Yen's algorithm:
    - reversal: path `1-5-2-3-4` has two reversals at `5` and `2`.
    - the `i`th iteration find the length of the shortest path from node `1` to node `k` among all paths have `i-1` or fewer reversals.
    - if the `i`th iteration does not update for some node, then it's converged; if convergence does not occur by `N`th iteration, negative cycle exists.
    - most efficient.

* All-pair shortest paths
    - Floyd
    - Dantzig: similar but longer to write

* Variants
    - value of path determined by the max/min one arc
    - value of path are product of values on arc
    - travel time on an arc determined by the start time
    - value of arc determined by the previous traveled arc
    - Dijkstra-like algorithm connecting two disjoint subset
