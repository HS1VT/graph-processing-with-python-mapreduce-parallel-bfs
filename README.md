# graph-processing-with-python-mapreduce-parallel-bfs

In this assignment, we will work with the road network in California. The data can be
downloaded from https://snap.stanford.edu/data/roadNet-CA.html . In this dataset,
intersections and endpoints in the city are represented by nodes and the roads
connecting these intersections or road endpoints are represented by undirected edges.
In total, the network contains 1965206 nodes and 2766607 edges.

● Task 1: Assume the weightage i.e. distance between any pair of nodes is 1.
In this scenario, write map-reduce jobs to find the shortest distance between a source
node and all other nodes.

● Task 2: Convert the graph into a weighted one in the following manner. For
every pair of nodes, <i,j> assign the distance between them as (((i+j)%20)+1). This will
give you a distance within the range of [1,20] between any two nodes. Now, in this
scenario, write map-reduce jobs to find the shortest distance between a source node
and all other nodes.

● Task 3: Randomly choose 1000 nodes from the network. Use these nodes as
source nodes and find the shortest distances from these nodes to all other nodes in the
network assuming the Task 1 setup. Also, calculate the time taken to complete the
map-reduce task for each of these 1000 nodes. Now, draw a scatter plot where in X axis,
you have the average shortest distances for each of the source nodes and in Y axis, you
have the corresponding time taken. Do we see any correlation there?

● Again, try the same with plotting the local clustering coefficients
(https://en.wikipedia.org/wiki/Clustering_coefficient#Local_clustering_coefficient) of the
nodes in the X axis and keeping the Y axis same as before. Do we see any correlation
there? If yes, why?

● Task 4: Update the Task 3 code in a manner such that we get
to know not only the shortest distance but also the shortest path between the source
node and every other node in the network. Or, if you think it cannot be done in the
Map-reduce setup, justify it.



Towards the end, we also used AWS EMR to compare the runtimes.
 
