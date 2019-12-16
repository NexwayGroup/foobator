# Tileswork

Write a function accepting two numbers being a dimension of a room, and another two numbers
being a dimension of a tile. Function should return number of tiles needed to cover the floor
area of a room.

Important caveat: if tile needs be cut and remaining part is at least the size of half
the tile, that remaining part should be reused if another half-or-less tile is required.

Bonus points for:
- writing unit tests for testing common cases
- turning the function into a working HTTP API server
- recognizing the big O complexity of a solution for space and computation
- using tail call optimization (even if your language does not support one)

Input used to validate the solution:
- 4, 5, 0.2, 0.25
- 4, 5, 0.3, 0.3
- 10, 10, 0.8, 0.8
- 10, 10, 0, 5
- 0, 10, 0.1, 0.1
- 10, 10, -0.5, 0.5
- -3, 4, 0.1, 0.1
