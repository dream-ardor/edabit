## Calculate Using String Operation

Create a function that takes two numbers and a mathematical operator and returns the result.
```c++
Examples

calculate(4, 9, "+") ➞ 13

calculate(12, 5, "-") ➞ 7

calculate(6, 3, "*") ➞ 18

calculate(25, 5, "/") ➞ 5

calculate(14, 3, "%") ➞ 2
```
### :fallen_leaf: My Code
```c++
int calculate(int a, int b, char c) {
  return c == '+' ? a+b : c == '-' ? a-b : c == '*' ? a*b : c == '/' ? a/b : a % b;
}
```
