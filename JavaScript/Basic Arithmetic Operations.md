## Basic Arithmetic Operations

Write a function that does the following for the given values: add, subtract, divide and multiply . This is simply referred to as the basic arithmetic operations. The variables have to be defined, but in this challenge, it will be defined for you. All you have to do, is to check the variables, do some string to integer conversion, use some if conditions, and apply the arithmetic operation.

The numbers and operation are given as a string and should result to an integer value.
```js
Examples
operation("1",  "2",  "add" ) ➞ 3

operation("4",  "5",  "subtract") ➞ -1

operation("6",  "3",  "divide") ➞ 2

Notes:

The numbers and operation are given as a string and should result to an integer value.
If the operation results to Infinity, then return "undefined" (e.g. division by zero).
Division results will be rounded down to its integral part.
```
### :leaves: My Code
```js
const operation = (a, b, c) => {
let a = +a , let b = +b;
 return a > 0 && b == '0' ? 'undefined' :
  c == 'add' ? a + b : c == 'divide' ? a / b :
  c == 'multiply' ? a*b : c == 'subtract' ? a-b : 0};
```
