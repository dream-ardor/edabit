## Stupid Addition
Create a function that takes two parameters and, if both parameters are strings, add them as if they were integers or if the two parameters are integers, concatenate them.
```js
Examples
stupidAddition(1, 2) ➞ 12

stupidAddition("1", "2") ➞ 3

stupidAddition("1", 2) ➞ null
```
```
Notes
If the two parameters are different data types, return null.
All parameters will either be strings or integers.
```
### :heavy_plus_sign: My Code
```js
const stupidAddition = (a, b) =>
 typeof a == 'string' && typeof b == 'string' ? +a + +b :
 typeof a == 'number' && typeof b == 'number' ? '' + a + b : null;
```
