## Even All the Way

Given an array of numbers, return an array which contains all the even numbers in the orginal array, which also have even indices.
```js
Examples
getOnlyEvens([1, 3, 2, 6, 4, 8]) ➞ [2, 4]

getOnlyEvens([0, 1, 2, 3, 4]) ➞ [0, 2, 4]

getOnlyEvens([1, 2, 3, 4, 5]) ➞ []
```
### :computer: My Code
```js
const getOnlyEvens = n => n.filter((a,b)=> a % 2 == 0 && b % 2 == 0);
```
