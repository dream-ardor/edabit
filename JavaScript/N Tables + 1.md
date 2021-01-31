## N Tables + 1

Create a function which takes a number n and prints out first 10 multiples of n with 1 added to it, separated by commas.
```js
Examples

nTablesPlusOne(7) ➞ 8,15,22,29,36,43,50,57,64,71

nTablesPlusOne(1) ➞ 2,3,4,5,6,7,8,9,10,11

nTablesPlusOne(3) ➞ 4,7,10,13,16,19,22,25,28,31
```
### :deciduous_tree: My Code
```js
const nTablesPlusOne = n => ''+[...Array(10)].map((_,i) => n * ++i + 1);
```
