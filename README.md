## Synopsis
A file contains the adjacency list representation of a simple undirected graph. There are
200 vertices labeled 1 to 200. The first column in the file represents the vertex label, and
the particular row (other entries except the first column) tells all the vertices that the
vertex is adjacent to. So for example, the 6th row looks like : "6  155 56  52  120 ......".
This just means that the vertex with label 6 is adjacent to (i.e., shares an edge with)
the vertices with labels 155,56,52,120,......,etc

The task here is to code up and run the randomized contraction algorithm for the min cut problem
and use it on the above graph to compute the min cut (e.g. 5) (HINT: Note this will have to include
an implementation of edge contractions. Initially, this can be done
naively, creating a new graph from the old every time there's an edge contraction. But there are also more efficient implementations.) 

(WARNING: Make sure to run the algorithm many times with different random seeds, and remember the
smallest cut found.)

## Motivation

The randomized contraction algorithm, an iterative algorithm which solves for the minimum cut in a graph, demonstrates the utility of randomization and iteration in algorithm writing. Optimization is crucial here as well, as implementations which take advantage of language features of C generally run much faster than implementations in Python, for example. This assignment also included preprocessing adjacency list files, creating Vertex and Graph classes, and practicing true randomization when choosing graph edges.  

## Acknowledgements

This algorithm is part of the Stanford University Algorithms 4-Course Specialization on Coursera, instructed by Tim Roughgarden.
