## Return the Total Number of Parameters

Create a function that returns the total number of parameters passed in.
```js
Examples
numberArgs("a", "b", "c") ➞ 3

numberArgs(10, 20, 30, 40, 50) ➞ 5

numberArgs(x, y) ➞ 2

numberArgs() ➞ 0
```

## My Code
```js
const numberArgs = (...args) => args.length;

```
