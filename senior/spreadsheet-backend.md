# Spreadsheet backend

Write a library acting as spreadsheet backend.

The following use cases should be supported:
- infinite number of rows and columns in document
- each cell may be either: blank, static text, or formula (cell starting with = sign)
- upon change of value all depending formulae in the document must be updated
- cell properties are: font, text size, text colour, background colour
- default cell properties inherited from document default
- selection ranges: rows, columns, rectangular selections inside document
- property change possible on cell as well as on selection range

Guidelines:
- follow SOLID principles
- identify design patterns where appropriate
- use git to track changes and maintain traceable commit history
- comment relevant pieces of code only
- do not store cells in database - keep them in memory for simplicity

Create sample test file and an example use of your library.
Bonus points for providing UML class diagram.
