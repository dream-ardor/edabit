## Buggy Code (Part 5)

Mubashir created an infinite loop! Help him by fixing the code in the code tab to pass this challenge (only syntax errors). Look at the examples below to get an idea of what the function should do.
```js
Examples
printArray(1) ➞ [1]

printArray(3) ➞ [1, 2, 3]

printArray(6) ➞ [1, 2, 3, 4, 5, 6]
```
### :leaves: My Code
```js
let printArray = n => [...Array(n)].map((a,b) => 1 + b);

let printArray = n => [...``.padStart(n, ` `)].map((a,i) => i+1);
```
