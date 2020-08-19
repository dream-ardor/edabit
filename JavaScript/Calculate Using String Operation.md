## Calculate Using String Operation

Create a function that takes two numbers and a mathematical operator and returns the result.
```js
Examples
calculate(4, 9, "+") ➞ 13

calculate(12, 5, "-") ➞ 7

calculate(6, 3, "*") ➞ 18

calculate(25, 5, "/") ➞ 5

calculate(14, 3, "%") ➞ 2
```
### :computer: My Code
```js
const calculate = (n1,n2,o) => eval(n1+o+n2);
```
