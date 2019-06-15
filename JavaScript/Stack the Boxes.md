## Stack the Boxes

Here's an image of four models. Some of the cubes are hidden behind other cubes. Model one consists of one cube. Model two consists of four cubes, and so on...

Write a function that takes a number n and returns the number of stacked boxes.
```js
Examples
stackBoxes(1) ➞ 1

stackBoxes(2) ➞ 4

stackBoxes(0) ➞ 0
```

## My Code
```js
const stackBoxes = n => Math.pow(n, 2);

```
