## How Many Digits?

Given an integer n . Your task is to find how many digits contains this integer without using String or Array methods!
```js
Examples
sumDigits(100) ➞ 3

sumDigits(1000) ➞ 4

sumDigits(1) ➞ 1
```
### :evergreen_tree: My Code
```js
const sumDigits = n => Math.ceil(Math.log10(n+1) || 1);
```
