# Bitcoin script

Develop library for running Bitcoin-like script.

Bitcoin script is a FORTH-like, stack-based, non Turing-complete language.
Program is list of operands and operators separated with space. Each item is put onto a stack
and if is a recognized token it is executed and its result it put back on a stack.
Initially, only develop putting string operands, and the following operations:
- OP_DUP should duplicate the topmost item on a stack
- OP_EQUALS should take two items off the stack and put back "1" if those are equal, "0" otherwise
- OP_SHA256 should take last item and put back its SHA256 hash
- . (single dot) should pop the topmost item and echo it to a screen

Consider the following scripts:
- `a30eaba820e49a95101a949ca387612b38424c34a8b6237c37eebcf055aac086 nexway OP_SHA256 OP_EQUALS .`
- `1111111111111111111111111111111111111111111111111111111111111111 nexway OP_SHA256 OP_EQUALS .`

Library must be open to extension with additional operations without requiring change
in existing code.

Use git to track changes. Comment relevant pieces of code only.
Use doc blocks to document parameters and return types.

Provide unit tests for critical parts, ideally for whole library.
Use Composer to manage dependencies to third party libraries.

Create sample test file and an example use of your library.

Afterwards, please add operation OP_IF to remove one item from the stack
and execute subsequent commands if its value was "1", and skip to matching
OP_ENDIF otherwise. OP_ENDIF should not pop from or push to stack any values.
Run the following scripts:

- `not a30eaba820e49a95101a949ca387612b38424c34a8b6237c37eebcf055aac086 nexway OP_SHA256 OP_EQUALS OP_IF successful OP_ENDIF .`
- `not 1111111111111111111111111111111111111111111111111111111111111111 nexway OP_SHA256 OP_EQUALS OP_IF successful OP_ENDIF .`

Commit your changes separately to create a tracable git history.
Don't squash commits together.