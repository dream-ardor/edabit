## Is the Number a Repdigit

A repdigit is a positive number composed out of the same digit.

Create a function that takes an integer and returns whether it's a repdigit or not.
```js
Examples
isRepdigit(66) ➞ true

isRepdigit(0) ➞ true

isRepdigit(-11) ➞ false
```
### :computer: My Code
```js
let isRepdigit = n => /^([0-9])\1*$/.test(n);
```
