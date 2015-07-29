# Leap years

Write a function that takes year as an int and returns boolean to indicate
if the year is a leap one. Do not use built-in PHP functions to detect leap year.
Provide basic protection against bogus parameters.

Comment relevant pieces of code only. Use doc blocks to document
parameters and return types.

Writing a unit tests for testing common cases is highly recommended
and will be rewarded with extra points.

The year is a leap year if:
- is evenly divisible by 4
- but is not evenly divisible by 100
- unless it is also evenly divisible by 400

Input used to validate the solution:
- 2016
- 2015
- 2000
- 1604
- 1603
- 1600
- 0
- -4
- -100
- -400
- -401
- "ABCDE"
- ""
- null
