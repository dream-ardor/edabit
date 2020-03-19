## Simple OOP Calculator

Create functions for the Calculator class that can do the following:
```js
Add two numbers.
Subtract two numbers.
Multiply two numbers.
Divide two numbers.

Examples:

var calculator = new Calculator()

calculator.add(10, 5) ➞ 15

calculator.subtract(10, 5) ➞ 5

calculator.multiply(10, 5) ➞ 50

calculator.divide(10, 5) ➞ 2
```
### :keyboard: My Code
```js
class Calculator {
  add = (a,b) => a + b;
  subtract = (a,b)=> a - b;
  multiply = (a,b)=> a * b;
  divide = (a,b)=> a / b;
}
```
