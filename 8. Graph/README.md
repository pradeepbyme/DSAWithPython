<h1>Graph - Data Strcture</h1>

Graphs are a fundamental data structure in computer science, often used to model relationships between entities. They consist of nodes (also called vertices) and edges that connect these nodes. Graphs are versatile and are applied across various fields, including social networks, navigation systems, and recommendation engines.

### Graph Components

*   **Vertices (Nodes)**: These represent entities or points in the graph. For example, each user in a social network graph is a vertex.
    
*   **Edges**: These are connections between vertices. An edge signifies a relationship or link between two vertices, like a "friendship" connection between users in a social network.
    
*   **Weight**: An optional attribute on edges, representing the cost or value associated with the connection (e.g., distance, time, or capacity).
    

### Types of Graphs

1.  **Directed Graphs (Digraphs)**: Each edge has a direction, going from one vertex to another. A directed edge from vertex A to vertex B does not imply a connection from B to A. These are used in scenarios where relationships are one-way, like web page links or follower relationships on Twitter.
    
2.  **Undirected Graphs**: Edges have no direction, so if there's an edge between A and B, it implies a two-way relationship. Undirected graphs model mutual relationships, like friendships or undirected connections.
    
3.  **Weighted Graphs**: Each edge has an associated weight. These are used in contexts like transportation networks, where distances or costs need to be considered.
    
4.  **Unweighted Graphs**: All edges are equal, without any associated cost or weight. Social networks and certain network structures can be represented as unweighted graphs.
    
5.  **Cyclic Graphs**: Graphs that contain at least one cycle, where you can start from a node and follow a series of edges to return to the same node. Cycles are common in directed graphs.
    
6.  **Acyclic Graphs**: Graphs without any cycles. A popular example is a tree, which is an acyclic, undirected graph. Directed Acyclic Graphs (DAGs) are used in applications like scheduling and dependency resolution.
    

### Graph Representation

Graphs can be represented in several ways:

1.  **Adjacency Matrix**: This is a 2D array where each cell (i, j) holds a value that indicates the presence (and possibly weight) of an edge from vertex i to vertex j. It’s efficient for dense graphs but can consume more memory.
    
2.  **Adjacency List**: Each vertex has a list (or dictionary) of adjacent vertices. This representation is memory-efficient and works well for sparse graphs. Most graph algorithms favor adjacency lists for their efficiency.
    
3.  **Edge List**: A list of edges, where each edge is represented as a pair or triplet (if weighted) of vertices. This representation is straightforward and compact for graph storage but not efficient for edge queries.
    

### Basic Operations on Graphs

1.  **Graph Traversal**
    
    *   **Breadth-First Search (BFS)**: Explores all nodes at the present "depth" level before moving on to nodes at the next depth level. It’s useful for finding the shortest path in an unweighted graph or for exploring all nodes reachable from a starting node.
        
    *   **Depth-First Search (DFS)**: Explores as far along each branch as possible before backtracking. DFS is useful for finding connected components, detecting cycles, and solving maze-like problems.
        
2.  **Pathfinding**
    
    *   **Single-Source Shortest Path**: Finds the shortest path from a source vertex to all other vertices. Common algorithms include Dijkstra's (for weighted graphs with non-negative weights) and Bellman-Ford (handles negative weights).
        
    *   **All-Pairs Shortest Path**: Calculates the shortest paths between every pair of vertices. Algorithms like Floyd-Warshall are used for this purpose but can be inefficient for large graphs.
        
3.  **Cycle Detection**
    
    *   In **directed graphs**, cycles can indicate problems in scheduling or dependency graphs, so detecting cycles is essential.
        
    *   In **undirected graphs**, cycle detection helps in identifying redundant paths or ensuring a graph is a tree. DFS and Union-Find are common techniques for cycle detection.
        
4.  **Connected Components**
    
    *   **Connected Component**: A subgraph in which any two vertices are connected directly or indirectly. In an undirected graph, connected components help in identifying isolated subgroups.
        
    *   **Strongly Connected Component**: In a directed graph, a strongly connected component is a maximal subset of vertices where every vertex is reachable from every other vertex in the subset. Algorithms like Kosaraju’s or Tarjan’s can identify these.
        
5.  **Minimum Spanning Tree (MST)**
    
    *   An MST is a subset of edges in a weighted undirected graph that connects all vertices without any cycles and with the minimum possible total edge weight.
        
    *   **Kruskal's Algorithm** and **Prim's Algorithm** are widely used to construct MSTs. MSTs are useful in network design, like laying out cables in an efficient way.
        
6.  **Topological Sorting**
    
    *   Applicable only to Directed Acyclic Graphs (DAGs), topological sorting arranges vertices in a linear order such that for every directed edge u -> v, vertex u comes before v.
        
    *   This is useful in scheduling and dependency management, like task scheduling, where some tasks must precede others.
        
7.  **Matching and Maximum Flow**
    
    *   **Matching**: In a bipartite graph, matching pairs of nodes such that no two edges share a node. Applications include job assignments, pairings in networks, etc.
        
    *   **Maximum Flow**: Finds the maximum possible flow from a source to a sink in a flow network. The Ford-Fulkerson and Edmonds-Karp algorithms are used to determine maximum flow, which has applications in network routing, resource allocation, and more.
        

### Applications of Graphs

Graphs are powerful tools for modeling relationships in real-world scenarios:

*   **Social Networks**: Nodes represent users, and edges represent friendships or follow relationships.
    
*   **Web Crawling**: Web pages as nodes and hyperlinks as directed edges; used in search engines.
    
*   **Navigation and Maps**: Cities as nodes and roads as weighted edges representing distances or travel times.
    
*   **Dependency Management**: Tasks in project planning, where edges represent dependencies.
    
*   **Computer Networks**: Routers/switches as nodes, and connections as edges.</br>


<b>Credits</b>: [Pradeep Rangisetti](https://www.linkedin.com/in/pradeepbyme)