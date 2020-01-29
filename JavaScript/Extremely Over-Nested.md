## Extremely Over-Nested

Create a function that returns the original value from a matrix with too many sub-arrays.
```js
Examples
deNest([[[[[[[[[[[[3]]]]]]]]]]]]) ➞ 3

deNest([[[[[[[true]]]]]]]) ➞ true

deNest([[[[[[[[[[[[[[[[["edabit"]]]]]]]]]]]]]]]]]) ➞ "edabit"
```
### :pencil2: My Code
```js
const deNest = a => a.flat(Infinity)[0];
```
