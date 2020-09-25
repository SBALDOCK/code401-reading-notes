## Graphs

* Graphs are non-linear data structures
* Even more confusing than previous data structures
* Collection of **vertices** (nodes), potentially connected by line segments called **edges**

#### Vocabulary

**Vertex** - Also called a node. A data object that can have zero or more adjacent vertices
**Edge** - Connection between two vertices
**Neighbor** - Adjacent nodes to a node, connected by an edge
**Degree** - Number of edges connected to a vertex

### Directed vs Undirected

**Undirected** - A graph where each edge is bi-directional, meaning the graph does not monve in any specific direction

**Directed** - Also called a **Digraph**, is a graph where every edge is directed. Each node is directed at another node. 

**Complete** - All nodes connected to all other nodes

**Connected** - All vertices/nodes have at least one edge - A **Tree** is a form of connected graph

**Disconnected** - Some vertices may not have edges

**Cycle** - When a node can be traversed through and potentially end up back at itself

**Acyclic** - A graph without cycles. An acyclic directed graph is called a **DAG**, and can be represented as a tree.

**Cyclic** - A graph with cycles. A cycle is a path of a positive length that starts and ends at the same vertex. 

**Adjacency Matrix** - Assigns a value based on whether a vertex connects to another vertex. Represented through a two-dimensional array

**Adjacency List**  - Most common way to represent graphs. A collection of linked lists or array that lists all of the other vertices that are connted. Makes it easy to view if one vertices connects to another

**Weighted Graph** - A graph with numbers assigned to its edges. Numbers are called weights. 

### Traversals

**Breadth First** - Start at a specific vertex/node, which must be specified. Visit all the nodes that are closest to the root as possible. Then traverse outwards, level by level, until all vertices are visted. Requires a flag that specifies if a node has already been visited to avoid an infinite loop. Upon each visit, set the "visited" flag from false to true. 
  * Disconnected nodes are not traversed
  * Outputs nodes that are connected in some relations to the root passed in

**Depth First** - Push root node into a stack, start while loop while stack is not empty, peek at the top node in the stack. If top notde has unvisited children, mark top node as visited, push any unvisited children back into the stack. If top node does not have unvisited children, pop node off the stack. Repeat until stack is empty. 

### Real World Uses

* GPS and Mapping
* Driving Directions
* Social Networks
* Airline Traffic
* Netflix uses graphs for suggestions of products

