# Wiki syntax

Write a library for converting Wiki syntax into HTML

Library should be open for extension if support for additional conversion
and formatting rules are needed.

Use the following formatting rules:
- Text wrapped with double star is `**bold**` - use HTML tag `<b>`
- Text enclosed with underscores is `_italic_` - use HTML tag `<i>`
- Mixing bold and italic should be allowed
- Line starting with four spaces is a preformatted text - use HTML tag `<pre>`
- Subsequent preformatted lines should form single preformatted block
- Line wrapped with equal signs should be made into a heading - use `<h1>`, `<h2>`, `<h3>` tags
- Heading level should depend on number of equal signs, i.e. `=== Hello ===` is `<h3>`

Development standard requirements:
- library must be open to extension with additional operations without requiring change
in existing code
- commit your changes separately to create a well organized git history

Bonus points for:
- writing unit tests for testing common cases
- turning the function into a working HTTP API server
