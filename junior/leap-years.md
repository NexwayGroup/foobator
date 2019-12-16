# Leap years

Write a function that takes year as an int and returns boolean to indicate
if the year is a leap one. Do not use built-in/stdandard library functions to detect leap year.
Provide basic protection against bogus parameters. Be wary that there is no year 0.

Bonus points for:
- writing unit tests for testing common cases
- turning the function into a working HTTP API server

The year is a leap year if:
- is divisible by 4
- but is not divisible by 100
- unless it is also divisible by 400

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
