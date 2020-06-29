## Multidimensional Array into Single Dimensional Array

Create a function that takes multidimensional array, converts into one dimensional array and returns it using Recursion.
```js
Examples
flatten([[17.2, 5, "code"]]) ➞ [17.2, 5, "code"]

flatten([[[[[2, 14, "rubber"]]], 2, 3, 4]])) ➞ [2, 14, "rubber", 2, 3, 4]

flatten([["balkot"]]) ➞ ["balkot"]

Notes:
Input contains at least one element.
Use of built in methods is discouraged.
```
### :computer: My Code
```js
const flatten = arr => 
 arr.reduce((acc, cur) => acc.concat(Array.isArray(cur) ? flatten(cur) : cur), []);
```
