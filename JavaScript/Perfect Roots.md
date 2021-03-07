## Perfect Roots

Given a number n, find if its 2nd, 4th and 8th roots are all integers (perfect roots), return true if it exists, false if not.
```js
Examples
perfectRoots(256) ➞ true
# 2nd root of 256 is 16
# 4th root of 256 is 4
# 8th root of 256 is 2

perfectRoots(1000) ➞ false

perfectRoots(6561) ➞ true
```
### :leaves: My Code
```js
const perfectRoots = n => n ** 0.5 % 1 == 0;


//alternate solution
const perfectRoots = n => Number.isInteger(Math.pow(n,1/2)) && Number.isInteger(Math.pow(n,1/4)) && Number.isInteger(Math.pow(n,1/8));

const perfectRoots = n => Math.sqrt(n) % 1 == 0;
```
