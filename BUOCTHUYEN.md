
# Exercise: TIE THE BOATS (BUOCTHUYEN)

## Problem Description

You are managing a dock that can hold up to **N boats**, numbered from `1` to `N`
(`1 ≤ N ≤ 250`).

To prevent the boats from drifting away, they are tied together using ropes.

There are **M ropes** connecting pairs of boats (`1 ≤ M ≤ N × (N − 1) / 2`).
Between any two boats, there is **at most one rope**.

Boat `1` is firmly tied to the dock using a chain.
Other boats must be connected to boat `1` through one or more ropes.
However, some boats may **not** be connected to boat `1` at all.

---

## Task

Determine which boats are **not connected** to boat `1`.

- Boat `1` is always considered connected to itself
- If all boats are connected to boat `1`, output `0`

---

## Input

Read from file `BTHUYEN.INP`:

- First line: two integers **N** and **M**
- The next **M lines** each contain two integers:

```
ti tj
```

Meaning boat `ti` is directly connected to boat `tj` by a rope

---

## Output

Write to file `BTHUYEN.OUT`:

- Output `0` if there are no boats disconnected from boat `1`
- Otherwise, output the **numbers of the disconnected boats** in increasing order,
  one number per line

---

## Example

### Input
```
6 4
1 3
2 3
1 2
4 5
```

### Output
```
4
5
6
```

---
