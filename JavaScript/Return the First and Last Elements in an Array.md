## Return the First and Last Elements in an Array

Create a function that takes an array of numbers and return the first and last elements as a new array.

Examples:

firstLast([5, 10, 15, 20, 25]) ➞ [5, 25]

firstLast(["edabit", 13, null, false, true]) ➞ ["edabit", true]

firstLast([undefined, 4, "6", "hello", null]) ➞ [undefined, null]

## My Code
```js
function firstLast(arr) {
  return ([arr.shift(), arr.pop()])
}
```
