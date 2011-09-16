The Cargo-Loading Problem
=========================

Introduction
------------

* Complete pack
    - Item `i`
    - Weight of item `w_i`
    - Value of item `v_i`
    - Capacity `w`

Algorithm 1
-----------

* Graph with `0..w` as vertexes.

* One kind of item is one kind of arc.

* Find longest path in the graph.

Algorithm 2
-----------

* Slightly improved version of algorithm 1, solution has unique representation, do not calculate one solution multiple times.

Algorithm 3
-----------

* _Forward-looking_ procedure, use permanent (optimal) value of `f(w)` to compute temporary values of `f(w)` for larger `w`.

Algorithm 4
-----------

* Use _breakpoints_.
