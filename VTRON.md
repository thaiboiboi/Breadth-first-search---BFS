
# Exercise: INTERSECTING CIRCLES (VTRON)

## Problem Description

On a two-dimensional plane, there are **N circles** `V1, V2, ..., VN`.

We construct a graph with **N vertices** (numbered from `1` to `N`), where:

- Each circle `Vi` corresponds to vertex `i`
- Two vertices are connected by an edge if the corresponding circles **intersect**
  (i.e. they have **exactly two common points**)

---

## Task

Determine the **minimum number of edges** in a path from **vertex 1** to **vertex N**.

If no such path exists, output `-1`.

---

## Input

Read from file `VTRON.INP`:

- The first line contains an integer **N** (`2 ≤ N ≤ 1000`) — the number of circles
- The next **N lines** each contain three integers:

```
x y r
```

Where:
- `(x, y)` are the coordinates of the **center** of the circle
- `r` is the **radius** of the circle

Constraints:
- `-10000 < x, y < 10000`
- `0 < r < 10000`

---

## Output

Write to file `VTRON.OUT`:

- The **minimum number of edges** from vertex `1` to vertex `N`
- Output `-1` if no path exists

---

## Notes

- The graph is **unweighted**
- Each edge represents one intersection between two circles
- To find the minimum number of edges, **Breadth-First Search (BFS)** should be used

---

## Example

### Input
```
3
0 0 1
4 0 4
1 0 2
```

### Output
```
2
```

