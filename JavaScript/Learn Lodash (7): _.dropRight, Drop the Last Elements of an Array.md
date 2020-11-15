## Learn Lodash (7): _.dropRight, Drop the Last Elements of an Array

According to the lodash documentation, _.dropRight Creates a slice of an array with n elements dropped from the end.

Here are some example intros:

Create a function that takes a number as an argument and returns "even" or "odd".
Create a function that takes an array of numbers and returns the smallest number in the set.
Create a function that takes a string and returns a string with its letters in alphabetical order.
```js
Examples
dropRight([1, 2, 3]) ➞ [1, 2]

dropRight([1, 2, 3], 2) ➞ [1]

dropRight([1, 2, 3], 5) ➞ []

dropRight([1, 2, 3], 0) ➞ [1, 2, 3]
```
### :leaves: My Code
```js
const dropRight = (a, n=1) =>  n > 0 ? a.slice(0,-n) : a;
```
