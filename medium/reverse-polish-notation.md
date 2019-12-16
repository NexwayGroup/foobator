# Reverse Polish Notation

Develop library for evaluating Reverse Polish Notation exprenssions

RPN is a notation of expressions without using parenthesis. Operands are read from input
and put on stack. Once operation is encountered, required number of operands are popped from stack
and passed to operation for processing. Then the resulting value is put back on stack.

Consider the following operations:
- `inc` (with 1 operand) - pops one operand, puts its value incremented by 1
- `add` (with 2 operans) - pops two operands, puts sum of them
- `dup` (with no operand) - pops one operand, puts the same value twice
- `avg` (with 1 + n operands) - pops first operand which tells how many more operand to pop (n), puts mean value of n operands

Development standard requirements:
- library must be open to extension with additional operations without requiring change
in existing code
- commit your changes separately to create a well organized git history

Bonus points for:
- writing unit tests for testing common cases
- turning the function into a working HTTP API server

Example input used for testing:
- `1 dup` = 1
- `2 2 add` = 4
- `0 inc inc inc` = 3
- `0 inc inc dup inc inc dup inc inc 3 avg` = 4
