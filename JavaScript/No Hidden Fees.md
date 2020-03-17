## No Hidden Fees

Given an array of prices prices and a "supposed" total t, return true if there is a hidden fee added to the total (i.e. the total is greater than the sum of prices), otherwise return false.
```js
Examples
hasHiddenFee(["$2", "$4", "$1", "$8"], "$15") ➞ false

hasHiddenFee(["$1", "$2", "$3"], "$6") ➞ false

hasHiddenFee(["$1"], "$4") ➞ true
```
### :herb: My Code
```js
const hasHiddenFee = (p, t) =>
 +p.map(x => +x.slice(1)).reduce((a,b) => a+b) < +t.slice(1);
```
