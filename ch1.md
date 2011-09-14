Elementary Path Problems
========================

Introduction
------------

* Definition: optimization procedure that is particularly applicable to problems requiring a sequence of interrelated decisions.

* Sequence of *decisions* to sequence of *situations*, to _optimize_ some measure of *value*.

A Simple Path Problem
---------------------

* Problem: one-way street, Manhattan-style city, from A to B.

The Dynamic-Programming Solution
--------------------------------

* Define sub-problems, solve the original problem by using the results from sub-problems.

* So we can solve all the sub-problems recursively in some order.

Terminology
-----------

* Define:
  * **optimal value function**: the rule that assigns values to various subproblems, it has **arguments**.
  * **optimal policy function**: the rule that associats the best first decision with each subproblem.
  * **recurrence relation**: a formula or set of formulas relating various values of _*OVF*_.
  * **boundary conditions**.

* Procedure:
  * To solve a problem by dynamic programming, we choose the arguments of the optimal value function and define that function to allow the use of the principle of optimality to write a recurrence relation.
  * Starting with the boundary conditions, we then use the recurrence relation to determine concurrently the optimal value and policy functions.
  * When the optimal value and decision are known for the value of the argument that represents the original whole problem, the solution is completed and the best path can be traced out using the optimal policy function alone.

Computational Efficiency
------------------------

* The time complexity of previous problem is `$O(N^2)$`.

Forward Dynamic Programming
---------------------------

* We can reverse the viewpoint of start point and end point, to obtain another representation of sub-problems. This is called _*forward* dynamic programming procedure_.

A More Complicated Example
--------------------------

* Problem: when turning in path requires additional cost.

Solution of the Example
-----------------------

* Solution: add one _argument_ to the _optimal value function_.

The Consultant Question
-----------------------

* The art of dynamic-programming formulation involves the proper choice of the arguments for the optimal value function.

* A good way to determin the right amount of arguments of _OVF_ is to think as "asking the consultant question."

Stage and State
---------------

* In _OVF_, the *monotonic* argument is called the *_stage_ variale*, all the others are called *_state_ variables*.

The Doubling-Up Procedure
-------------------------

* Usually, the cost of a certain step _do not depend_ on the stage/time.

* The doubling-up procedure is that the stage `$M+N$` depends on stage `$M$` and stage `$N$`.
