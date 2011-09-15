The Traveling-Salesman Problem
==============================

Introduction
------------

* Definition: a minimum-cost tour traveling all `N` vertexes and returning to start.

Dynamic-Programming Formulation
-------------------------------

* `f_i(j,S)` = the length of the shortest path from city `1` to city `j` via the set of `i` intermediate cities `S`

* Complexity `N^2 * 2^N`.

A Doubling-Up Procedure for the Case of Symmetric Distances
-----------------------------------------------------------

* When the distance matrix of graph is a symmetric, assume `N` is even, we can solve all `f_i(j,S)` where `i <= (N-2)/2`, then combine complement two of them.

* Significantly reduced computing time.

Other Versions of the Traveling-Salesman Problem
------------------------------------------------

* Variant 1: without returning to city 1.

* Variant 2: visit other vertexes at least once, not exactly once.

* Exercises:
    - diffferent variants of values on arc
    - adding requirements "city `i` must preced `j`"
    - use `O(2^N)` Dijkstra-like labels to solve the original problem
