## Nth Star Number

Create a function that takes a positive integer and returns the nth "star number".

A star number is a centered figurate number a centered hexagram (six-pointed star), such as the one that Chinese checkers is played on.
```js
Examples
starNumber(2) ➞ 13

starNumber(3) ➞ 37

starNumber(5) ➞ 121
```
### :star: My Code
```js
const starNumber = n => 6 * n * (n - 1) + 1;
```
