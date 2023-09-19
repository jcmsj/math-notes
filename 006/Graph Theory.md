# Graph Theory

1. Vertex
2. Edge
3. Parallel edge - two or more edges incident to the same two vertices.
4. Loops - An edge starts and ends with the same vertex.

## Types

### Multigraph
* Has no loops.

### Pseudograph
* Has at least one loop.

### Simplegraphs
* No parallel edges and no loops.

### Complete graph
* K<sub>n</sub> has n vertices where every pair of vertices is joined by one edge.
* __Trivial Graph__ - K<sub>1</sub> with one vertex and no edge.

### Directed graph
* Has arcs

#### In-degree & Out-degree of vertex v
* Must be a directed graph
* __Terminal vertex__ -  the direction an edge is pointing at.
* __deg<sup>-</sup>(v)__ - number of edges with terminal vertex v. Read as In-degree
* __Initial vertex__ - the direction an edge originates.
* __deg<sup>+</sup>(v)__ - number of edges with initial vertex v. Read as "out-degree
* With loops - adds one to In/out-degree.

#### Handshaking algorithm (lemma)
* edge count = summation d(v) = 2m
* edge count = Twice the sum of degrees.
### Adjacent and Incident
* If e = {u,v} E E(G), vertices u and v are said to be adjacent to each other and incident to e.

### Underlying Graph
* Directed graph -> Complete graph.
* Replace arcs into edges

### Tournament
* Complete graph -> Directed graph

## Properties
### Degree of a vertex
* deg(v) = Number of edges incident with vertex v.
* Loop at a vertex contributes twice to the degree.

### Pendant and Isolated Vertex
* Pendant = deg(v) == 1
* Isolated vertex = deg(v) == 0

### Regular graph
* Each vertex has the same degree.
* All complete graphs are regular graphs but not vice versa.
* Julius Peter Christian Petersen - 
  
### Subgraph
* Like subset
* A graph's vertices belongs to V(G) and each edge belong to E(G).

### Bipartite Graph
* A graph G whose vertex set could be split into two disjoint sets A,B so that each edge G joins a vertex of A and a vertex B.
* A,B's veetices are usually colored differently.
* Complete bipartite
  * Each vertex in A is joined to each vertex in B by just one edge.
  * Denoted as K<sub>k,s</sub> with r for black vertices and s for white vertices.
## Theorems

##
Let G:simple graph with at least 2 vertices. Then G has at least 2 vertices with the same degree.

## Corollary
* 1.1. Handshaking algo -> even number
* 1.2: In G, the number of instances of odd degrees is even.

## Walk
* a finite or infinite sequence of edges that joins a sequence of vertices.
* v<sub>0</sub>-> v<sub>1</sub>->...v<sub>n</sub>
* __Closed walk__ - walks ends at v<sub>0</sub>.
* __Open walk__ - !closed walk.
* __Trail__ - Walk with distinct edges.
* __Path__ - is a trail in which all vertices (and therefore also all edges) are distinct.
* __Circuit__ - Nontrivial closed trail from vertex v to itself.
* __Cycle__ - A circuit with no reptitions except a start/end vertices.

| Type        | vertices                      | Edges      | Extra                           |
| ----------- | ----------------------------- | ---------- | ------------------------------- |
| Walk        | Repeatable                    | Repeatable |                                 |
| Closed Walk | Walk with same start and end. | Repeatable | Walk                            |
| Trail       | Repeatable                    | Unique     | walk                            |
| Path        | Unique  except start and end. | Unique     | Path                            |
| Circuit     | Repeatable                    | Unique     | Nontrivial closed trail         |
| Cycle       | Unique except start and end.  | Unique     | Simple Circuit / Closed Circuit |

## Trees
A graph with:
1. Undirected
2. Connected - any two vertices connected by one edge.
3. Acyclic - 

* __Bridge__ - Edge when removed the graph becomes disconnected.
* __Forest__ - Set of more than one tree.
  * c(G) = number of trees
  * c means component.