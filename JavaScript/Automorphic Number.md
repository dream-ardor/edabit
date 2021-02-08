## Automorphic Number

A number is called Automorphic number if its square ends in the same digits as the number itself. Create a function which takes a number n and returns true if it is an Automorphic number, otherwise false.
```js
Examples
automorphic(1) ➞ true

automorphic(3) ➞ false
// 3^2 = 9

automorphic(6) ➞ true
// 6^2 = 36 (ends with 6)
```
### :leaves: My Code
```js
const automorphic = n => String(n**2).endsWith(String(n));


//alternate solutions
const automorphic = n => (''+ n ** 2).endsWith(n)

const automorphic = n => `${n ** 2}`.endsWith(n);
```
