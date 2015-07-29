# Spreadsheet backend

Write a library acting as spreadsheet backend. The following use cases
should be supported:
- infinite number of rows and columns in document
- each cell may be: blank, static text, or formula
- upon change of value all depending formulae in the document must be updated
- cell properties are: font family, size, colour, background, bold flag, italic flag
- default properties inherited from document
- property change on selection (selected rows, selected columns, rectangular selections)

In addition, provide model documentation in UML Class Diagram and suite of unit tests
with near full code coverage.

Guidelines:
- follow SOLID principles
- identify design patterns where appropriate
- use git to track changes and maintain traceable commit history
- comment relevant pieces of code only
- use doc blocks to document parameters and return types
- use Composer to manage dependencies to third party libraries

Create sample test file and an example use of your library.
