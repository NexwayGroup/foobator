# Tileswork

Write a function accepting two numbers beind dimension of a room, and other two numbers
being dimension of a tile. Function should return number of tiles needed to cover the floor
area of a room.

Important caveat: if tile needs be cut and remaining part is at least the size of half
the tile, that remaining part should be reused if another half-or-less tile is needed.

Provide some protection against bogus parameters.

Comment relevant pieces of code only. Use doc blocks to document
parameters and return types.

Writing a unit tests for testing common cases is highly recommended
and will be rewarded with extra points.

Input used to validate the solution:
- 4, 5, 0.2, 0.25
- 4, 5, 0.3, 0.3
- 10, 10, 0.8, 0.8
- 10, 10, 0, 5
- 0, 10, 0.1, 0.1
- 10, 10, -0.5, 0.5
- -3, 4, 0.1, 0.1
- "3m", "4m", 0.1, 0.1
- 3, 4, null, false
