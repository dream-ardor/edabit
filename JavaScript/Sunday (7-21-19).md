## Equality of 3 Values
Create a function that takes three integer arguments (a, b, c) and returns the number of equal values.
```js
Examples
equal(3, 4, 3) ➞ 2

equal(1, 1, 1) ➞ 3

equal(3, 4, 1) ➞ 0
```
### :cherries:My Code
```js
const equal = (a, b, c) =>  a == b && a == c ? 3 : a == c || a == b ? 2 : 0;
```

## Fix the Error: Flattening an Array
I'm trying to write a function to flatten an array of subarrays into one array. (Suppose I am unware there is a .flat() method in the Array prototype). In other words, I want to transform this: [[1, 2], [3, 4]] into [1, 2, 3, 4].

Here is my code:
```js
function flatten(arr) {
  arr2 = [];
  for (let i = 0; i < arr.length; i++) {
    arr2.concat(arr[i]);
  }
  return arr2;
}
```
But...it doesn't seem to be working! Fix my code so that it correctly flattens the array.
```js
Examples
flatten([[1, 2], [3, 4]]) ➞ []
// Expected: [1, 2, 3, 4]

flatten([["a", "b"], ["c", "d"]]) ➞ []
// Expected: ["a", "b", "c", "d"]

flatten([[true, false], [false, false]]) ➞ []
// Expected: [true, false, false, false]
```
### :grapes:My Code
```js
const flatten = arr =>[].concat(...arr); 
```

## Hitting the Jackpot
Create a function that takes in an array (slot machine outcome) and returns true if all elements in the array are identical, and false otherwise. The array will contain 4 elements.
```js
Examples
testJackpot(["@", "@", "@", "@"]) ➞ true

testJackpot(["abc", "abc", "abc", "abc"]) ➞ true

testJackpot(["SS", "SS", "SS", "SS"]) ➞ true

testJackpot(["&&", "&", "&&&", "&&&&"]) ➞ false

testJackpot(["SS", "SS", "SS", "Ss"]) ➞ false
```
### :watermelon:My Code
```js
const testJackpot = r => r.every(v => v === r[0]);
```

## Factorize a Number
Create a function that takes a number as its argument and returns an array of all its factors.
```js
Examples
factorize(12) ➞ [1, 2, 3, 4, 6, 12]

factorize(4) ➞ [1, 2, 4]

factorize(17) ➞ [1, 17]
```
### :pineapple:My Code
```js
function factorize(num) {
  let arr = [];
   for(i=0; i<=num; i++) {
    if(num % [i] === 0) {
    arr.push(i)
  }
 }
  return arr;
}
```
## Xs and Os, Nobody Knows
Create a function that takes a string, checks if it has the same number of x's and o's and returns either true or false.

Return a boolean value (true or false).
The string can contain any character.
When no x and no o are in the string, return true.
```js
Examples
XO("ooxx") ➞ true

XO("xooxx") ➞ false

XO("ooxXm") ➞ true
// Case insensitive.

XO("zpzpzpp") ➞ true
// Returns true if no x and o.

XO("zzoo") ➞ false
```
### :peach:My Code
```js
const XO = str => str.replace(/[^x]/gi,'').length === str.replace(/[^o]/gi,'').length;
```


