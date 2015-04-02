# Wiki syntax

Write a library for converting Wiki syntax into HTML.

Library should be open for extension if support for additional conversion
and formatting rules are needed. In such case no modification to existing
code is permitted.

Use the following formatting rules:
- Text wrapped with double star is **bold** - use HTML tag <b>
- Text enclosed with underscores is italic - use HTML tag <i>
- Mixing bold and italic should be allowed
- Line starting with four spaces is a preformatted text - use HTML tag <pre>
- Subsequent preformatted lines should form single preformatted block

Use git to track changes. Comment relevant pieces of code only.
Use doc blocks to document parameters and return types.

Provide unit tests for critical parts, ideally for whole library.
Use Composer to manage dependencies to third party libraries.

Create sample test file and an example use of your library.

Afterwards, please add one more formatting rule:
- Line wrapped with equal signs should be made into a heading - use <h1>, <h2>, <h3> tags
- Heading level should depend on number of equal signs, i.e. === Hello === is <h3>

Commit your changes separately to create a tracable git history.
Don't squash commits together.