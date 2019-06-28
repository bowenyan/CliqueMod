# CliqueMod

It's a community detection algorithm for unweighted, undirected networks. It is a simple algorithm to detect disjoint communities in networks by merging cliques, but performs better than most of modularity-based community detection algorithm.

Find the detail vis these links:
https://ieeexplore.ieee.org/abstract/document/5358036
OR https://arxiv.org/pdf/1202.0480.pdf

To run it:

   java -cp CM.jar CM networkFile -m method -c nComm
  
where networkFile is the file containing the network, in "list of edges" format, method is the clique-finding algorithm to use ("BK" or "KJ"), and nComm is the number of communities required.

The program prints the modularity of the solution and outputs the solution to a file named "ClustersOutput.txt".
