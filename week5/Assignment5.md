# Assignment 5: Graph Analysis

For this assignment please refer to this input file: adj.txt.
Write a script that can accept an adjacency matrix as input, and construct a node-based representation of a graph. Next, write a method that takes two nodes as arguments, n1 and n2, and returns the number of nodes that are equidistant from n1 and n2. These are the nodes for which the shortest paths to n1 and n2 have the same length. Hint: run two breadth-first searches, one from n1 and one from n2.
The file adj.txt contains an adjacency matrix representing a graph with 25 nodes. Node 0 is represented by the first column and the first town, node 1 by the second column and the second row, and so forth. Use your script to compute the following:

1. Find the number of nodes equidistant to node 0 and node 1.

2. Find the number of nodes equidistant to node 0 and node 5.

3. Find the number of nodes equidistant to node 1 and node 8.
