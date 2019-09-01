## Probabilities (Part 1)
Given an array of numbers and a value n, write a function that returns the probability of choosing a number greater than or equal to n from the array. The probability should be expressed as a percentage, rounded to one decimal place.
```js
Examples
probability([5, 1, 8, 9], 6) ➞ 50.0

probability([7, 4, 17, 14, 12, 3], 16) ➞ 16.7

probability([4, 6, 2, 9, 15, 18, 8, 2, 10, 8], 6) ➞ 70.0
```
### :classical_building: My Code
```js
const probability = (a, n)=> 
 +(a.filter(x => x >= n).length / a.length * 100).toFixed(1);
```
