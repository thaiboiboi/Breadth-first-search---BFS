Exercise 1: CASTLE (File name: Castle.*)

A castle is represented as a rectangular grid with N rows and M columns.
Each cell is considered a room.

Two rooms are adjacent if they share a common side.
Each room may have from 1 to 4 two-way doors connecting it to its adjacent rooms.

In each room, there is a 4-bit binary number b3 b2 b1 b0 describing the state of its doors:

b0 = 0 ⇔ there is a door on the left side

b1 = 0 ⇔ there is a door on the top side

b2 = 0 ⇔ there is a door on the right side

b3 = 0 ⇔ there is a door on the bottom side

If a bit equals 1, that side is a wall and cannot be passed through.

Examples

Binary 1010 → doors on the left and right, walls on top and bottom

Binary 0100 → doors on left, top, bottom, wall on right

From one room, you can reach another room by passing through a sequence of doors.
A room group is defined as a set of rooms that are all reachable from one another.

Requirements

Given the binary values of all rooms in the castle, determine:

The number of room groups in the entire castle

The size of the largest room group (number of rooms)

# Input (Castle.INP)

First line: two positive integers N, M (1 ≤ N, M ≤ 100)

Next N lines: each line contains M integers
Each integer is the decimal representation of a 4-bit binary number describing a room

# Output (Castle.OUT)

Line 1: number of room groups

Line 2: size of the largest room group
