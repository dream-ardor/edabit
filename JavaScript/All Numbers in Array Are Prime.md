## All Numbers in Array Are Prime

Create a function thats takes an array of integers and returns true if every number is prime. Otherwise, return false.
```js
Examples
allPrime([7, 5, 2, 4, 6]) ➞ false

allPrime([2, 3, 5, 7, 13, 17, 19, 23, 29]) ➞ true

allPrime([1, 5, 3]) ➞ false
```
### :computer: My Code
```js
const allPrime = n => n.every(a => !'1'.repeat(a).match(/^1?$|^(11+?)\1+$/));
```
