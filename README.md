# CliqueMod

It's a community detection algorithm for unweighted, undirected networks. It is a simple algorithm to detect disjoint communities in networks by merging cliques, but performs better than most of modularity-based community detection algorithm.

Find the detail of the paper: [Detecting Communities in Networks by Merging Cliques](https://ieeexplore.ieee.org/abstract/document/5358036) or [arXiv:1202.0480](https://arxiv.org/pdf/1202.0480.pdf)

To run it:

   java -cp CM.jar CM networkFile -m method -c nComm
  
where networkFile is the file containing the network, in "list of edges" format, method is the clique-finding algorithm to use ("BK" or "KJ"), and nComm is the number of communities required.

networkFile format:

node1 node2

node1 node3
...

The program prints the modularity of the solution and outputs the solution to a file named "ClustersOutput.txt".
