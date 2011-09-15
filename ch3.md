Resource Allocation
===================

The Simplest Model
------------------

* Not really _dynamic_ (i.e. requiring a _sequence_ of decisions).

* `X` units of a resourse to be distributed among `N` activities. Each activity has a return function `r_i(x)`. How to allocate the resourse to maximize the total return?

Dynamic-Programming Formulation
-------------------------------

* To use dynamic programming, we view the solution set as stages.

Numerical Solution
------------------

Miscellaneous Remarks
---------------------

* This problem can be represent as a longest-path problem.

* Variants:
    - forward DP procedure
    - return function not monotonic
    - doubling-up procedure when activities have the same return function
    - two- or three-dimentional resource
    - additional requirement: total allocation for a subset have a lower limit
    - additional requirement: at most `M` of the allocations may be nonzero
    - additional requirement: if `k` activities are nonzero, a cost `h(k)` is assessed.
    - two kinds of return: money and public goodwill, maximize money while goodwill has a lower limit.

Unspecified Initial Resources
-----------------------------

* Two kinds of resource which have unit costs, initially given money, how to buy resources and allocate them optimally.

* Variant: three kinds of resource.

Lagrange Multipliers
--------------------

* TODO: it's so brand new...

Justlflcatlon of the Procedure
------------------------------

* TODO: skipped

Geometric Interpretation of the Procedure
-----------------------------------------

* TODO: skipped

Some Additional Cases
---------------------

* TODO: skipped

More Than Two Constraints
-------------------------

* TODO: skipped
