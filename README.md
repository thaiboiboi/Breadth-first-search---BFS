# Full of exercise I made to solve with BFS/DFS in C++
# BFS and DFS — Graph Traversal Algorithms

## Breadth-First Search (BFS)

**Breadth-First Search (BFS)** explores a graph **level by level**, starting from a given source node.

- Uses a **queue**
- Visits all neighboring nodes before moving deeper
- Guarantees the **shortest path** in an unweighted graph

**Common applications:**
- Shortest path in unweighted graphs
- Level-order traversal
- Finding connected components

**Time Complexity:** `O(V + E)`

---

## Depth-First Search (DFS)

**Depth-First Search (DFS)** explores a graph by going **as deep as possible** before backtracking.

- Uses **recursion** or a **stack**
- Fully explores one path before trying another
- Does **not** guarantee the shortest path

**Common applications:**
- Finding connected components
- Cycle detection
- Topological sorting

**Time Complexity:** `O(V + E)`

---

## Key Differences

| BFS | DFS |
|----|----|
| Uses a queue | Uses a stack / recursion |
| Level-by-level traversal | Deep-first traversal |
| Finds shortest path (unweighted) | No shortest-path guarantee |
