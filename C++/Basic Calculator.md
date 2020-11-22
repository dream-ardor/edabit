## Basic Calculator

Create a function that takes two numbers and a mathematical operator + - / * and will perform a calculation with the given numbers.
```c++
Examples
calculator(2, '+', 2) ➞ 4

calculator(2, '*', 2) ➞ 4

calculator(4, '/', 2) ➞ 2
```
### :maple_leaf: My Code
```c++
int calculator(int a, char c, int b) {
  return c == '-' ? a - b : c == '+' ? a + b : c == '*' ? a * b : a / b;
}
```
