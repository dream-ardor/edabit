## Reverse Coding Challenge #3

This is a reverse coding challenge. Normally you're given explicit directions with how to create a function. Here, you must generate your own function to satisfy the relationship between the inputs and outputs.

Your task is to create a function that, when fed the inputs below, produce the sample outputs shown.
```js
Examples:

[5, 7, 8, 2, 1], 2 ➞ [1, 1, 0, 0, 1]

[9, 8, 16, 47], 4 ➞ [1, 0, 0, 3]

[17, 11, 99, 55, 23, 1], 5 ➞ [2, 1, 4, 0, 3, 1]

[6, 1], 7 ➞ [6, 1]

[3, 2, 9], 3 ➞ [0, 2, 0]

[48, 22, 0, 19, 33, 100], 10 ➞ [8, 2, 0, 9, 3, 0]
```

## My Code
```js
const mysteryFunc = (arr, num) => arr.map(x => x % num);

```

## Analysis
Looking at the examples, it becomes clear that the output array is a result of taking the initial array and dividing it by the provided number and displaying the remainder of each given number. This can be accomplished by creating a function that maps over the initial array and uses the modulo operator against the given number in argument two.
