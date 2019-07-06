## Transforming Words into Binary Strings
Write a function that transforms all letters from [a,m] to 0 and letters from [n,z] to 1 in a string.
```js
Examples
convertBinary("house") ➞ "01110"

convertBinary("excLAIM") ➞ "0100000"

convertBinary("moon") ➞ "0111"
```
### :confetti_ball:My Code
```js
const convertBinary = str => 
str.replace(/[a-m]/gi, "0").replace(/[n-z]/gi, "1");

```
