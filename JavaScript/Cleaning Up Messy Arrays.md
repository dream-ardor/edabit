## Cleaning Up Messy Arrays

Create a function that takes an array as a parameter. This array will contain numbers represented as strings.

Your function should split this array to two new arrays. First array should contain only even numbers. The second only odd. Then, wrap these two arrays in one main array and return it.

Return empty array if there are no even numbers, or odd.
```js
Examples
['8'] ➞ [[8], []]
['7', '4', '8'] ➞ [[4, 8], [7]]
['11'] ➞ [[], [11]]
['9', '4', '5', '8'] ➞ [[4, 8], [9, 5]]
```
### :herb: My Code
```js
const cleanUpArray = a => [a.filter(b => b % 2 == 0).map(c => +c), a.filter(b=>b % 2).map(c => +c)];
```
