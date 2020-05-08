## Ones and Zeroes

Write a function that returns true if every consecutive sequence of ones is followed by a consecutive sequence of zeroes of the same length.
```js
Examples
sameLength("110011100010") ➞ true

sameLength("101010110") ➞ false

sameLength("111100001100") ➞ true

sameLength("111") ➞ false
```
### :computer: My Code
```js
const sameLength = s => s.match(/1+0*/g).every(a => !(a.length % 2));

```
