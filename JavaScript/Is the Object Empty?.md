## Is the Object Empty?

Write a function that returns true if an object is empty, and false otherwise.
```js
Examples:
isEmpty({}) ➞ true

isEmpty({ a: 1 }) ➞ false
```

## My Code
```js
const isEmpty = obj => Object.keys(obj).length === 0 ? true : false;


```
