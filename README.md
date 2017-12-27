# Analysis-of-vertex-cover-algorithms.
Analysis of 3 vertex cover algorithms has been done and written in c++.

Coding part:

Multithreading has been used. 4 threads has been implemented one forI/O, and one each for the
different approaches to solve the minimum vertex cover problem.

All three algorithms are explained below

Algo 1.REDUCTION-TO-CNF-SAT approach is used to find minimum vertex cover,using MiniSat SAT solver.Create a polynomial reduction of the decision version of VERTEX COVER to CNF-SAT.And these CNF-clauses are then send as an input to the Minisat,which provide result as sat or unsat.

Algo 2.Pick a vertex of highest degree (most incident edges). Add it to your vertex cover and
throw away all edges incident on that vertex. Repeat till no edges remain. We will call
this algorithm APPROX-VC-1.

Algo 3.Pick an edge hu, vi, and add both u and v to your vertex cover. Throw away all edges
attached to u and v. Repeat till no edges remain. We will call this algorithm APPROX-
VC-2.

Given a graph as input, program should output the vertex cover computed by each approach
in sorted order. That is, give the following input:

V 5
E {<2,1>,<2,0>,<2,3>,<1,4>,<4,3>}

The output from program will be 

1CNF-SAT-VC: 2,4
APPROX-VC-1: 2,4
APPROX-VC-2: 0,2,3,4

That is, the name of the algorithm, followed by a colon ’:’, a single space, and then the computed result as a sorted sequence of vertices, separated by commas.

Report Part:

The main part of report are graphs (plots) corresponding to the data  generated as described in the “Analysis” section above. One way to show the output is to have two plots: one for running times and the other for approximation ratio. The horizontal axis is the number of vertices. Plot the mean for each value of |V | for which we have made measurements, and the standard deviation as a yerrorbar. An example of a possible plot is shown in Figure 1. The remainder of report should be reasoning about plots. That is, explain why plots look the way they do. 
