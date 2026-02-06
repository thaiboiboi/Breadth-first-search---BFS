
# Exercise: SQUARES (HINHVUONG)

## Problem Description

On a two-dimensional plane, there are **N squares** `H1, H2, ..., HN` whose sides are parallel to the coordinate axes.

We construct a graph with **N vertices** (numbered from `1` to `N`), where:

- Each square `Hi` corresponds to vertex `i`
- Two vertices are connected by an edge **if and only if** the corresponding squares **overlap** (one square intersects the other)

---

## Task

Determine the **minimum number of edges** in a path from **vertex 1** to **vertex N**.

If no such path exists, output `-1`.

---

## Input

The input is read from file `HINHVUONG.INP`:

- The first line contains an integer **N** (`2 ≤ N ≤ 1000`) — the number of squares
- The next **N lines** each contain three integers:

```
xM yM d
```

Where:
- `(xM, yM)` are the coordinates of the **center** of the square
- `d` is the distance from the center to one side of the square

Constraints:
- `-100000 ≤ xM, yM ≤ 100000`
- `1 ≤ d ≤ 100000`

---

## Output

Write to file `HINHVUONG.OUT`:

- The **minimum number of edges** in a path from vertex `1` to vertex `N`
- Output `-1` if no path exists

---

## Notes

- The graph is **unweighted**
- Each edge represents one move between overlapping squares
- To find the minimum number of edges, **Breadth-First Search (BFS)** is the appropriate algorithm

---

## Example

### Input
```
3
0 0 1
1 0 1
4 0 2
```

### Output
```
2
```

---

