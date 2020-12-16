## Many Operators!

Some basic arithmetic operators are +, -, *, /, and %. In this challenge you will be given three parameters, num1, num2, and an operator op. Use the operator on number 1 and 2.
```c++
Examples

operate(1, 2, "+") ➞ 3
// 1 + 2 = 3

operate(7, 10, "-") ➞ -3
// 10 - 7 = -3

operate(20, 10, "%") ➞ 0
// 20 % 10 = 0
```
### :leaves: My Code
```c++
#define operate(a,b,c)c == '+' ? a + b : c == '-' ? a - b : c == '*' ? a * b : c == '/' ? a / b : a % b 
```
