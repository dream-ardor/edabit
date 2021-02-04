## A Simple Task

Create a function which takes a number n and return its decimal part.
```js
Examples
decimalPart(1.2) ➞ 0.2

decimalPart(-3.73) ➞ 0.73

decimalPart(10) ➞ 0
```
### :leaves: My Code
```js
const decimalPart = n => Math.abs(n % 1);
```
