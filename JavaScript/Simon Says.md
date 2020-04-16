## Simon Says

Create a function that takes in two arrays and returns true if the second array follows the first array by one element, and false otherwise. In other words, determine if the second array is the first array shifted to the right by 1.
```js
Examples
simonSays([1, 2], [5, 1]) ➞ true

simonSays([1, 2], [5, 5]) ➞ false

simonSays([1, 2, 3, 4, 5], [0, 1, 2, 3, 4]) ➞ true

simonSays([1, 2, 3, 4, 5], [5, 5, 1, 2, 3]) ➞ false
```
### :computer: My Code
```js
const simonSays= (a1, a2) => a1[0] == a2[1];
```
