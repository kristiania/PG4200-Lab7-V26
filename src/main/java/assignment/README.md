Lab pratice 7
=============

DFS - recursive depth first search 
-----------------------------------

> All tasks are completed within this `assignment`-package

task0 : Adjacency List Implementation of a Graph
------------------------------------------------

The _SimpleGraphDFS_ application reads an edge-list from a file and constructs a Graph. 
The Graph is stored as _AdjacencyMapGraph_. 
The application simply prints all the vertices followed by all the edges. 
The folder _files_ contains two graph files which you can use as input for the application:
_graph.txt_ and _graph2.txt_
Define a new graph in a textfile in _files_ and print it with the application.
Hint: we used the one graph in today's Lecture.


task1 : Recursive DFS
-------------------------------

Your task is to complete the recursive implementation of 
Depth First Search in _SimpleGraphDFS_ code line 112.

> First study the book

Study the code which is taken from Goodrich et al. Implementation  in the 6th edition of Data Structures and algorithms in java:

- you can read p. 592-598 for DFS
- on p. 588-591 you find the _AdjacencyMapGraph_ implementation of the _Graph_ ADT.
  

> Second study the code in _net.datastructures_

_AdjacencyMapGraph_ and all necessary classes are all part of the _net.datastructures_ package.
Notice that the adjacency lists are implemented in the inner class _MyVertex_ and the references from the edges in the inner class _MyEdge_.
The _Graph_ ADT does not define any traversal method.
You are supposed to implement your own Depth-First Search
  inside the class SimpleGraphDFS, in order to print its vertices in a depth-first search manner. 

  
> Third Printing with Depth-First Search  

The program _SimpleGraphDFS_ has a routine _void printDFS( String vert )_ that calls _DFS(graph,v)_ which currently does nothing. 
Please implement the method _DFS(graph,v)_ with a recursive implementation of Depth-first Search --
Study today's Graph Traversals slides for the pseudocode and examples. 
The routine should print the vertices as they are visited by the traversal: once when they are first visited and a second time when a vertex is finished. 
In order to do that, auxiliary methods _startVisit(v)_ and _finishVisit(v)_
are provided.

