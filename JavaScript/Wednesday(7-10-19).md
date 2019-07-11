## First and Last Index
Given a word, write a function that returns the first index and the last index of a character.
```js
Examples
charIndex("hello", "l") ➞ [2, 3]
// The first "l" has index 2, the last "l" has index 3.

charIndex("circumlocution", "c") ➞ [0, 8]
// The first "c" has index 0, the last "c" has index 8.

charIndex("happy", "h") ➞ [0, 0]
// Only one "h" exists, so the first and last index is 0.

charIndex("happy", "e") ➞ undefined
// "e" does not exist in "happy", so we return undefined.
```
Notes
- If the character does not exist in the word, return undefined.
- If only one instance of the character exists, the first and last index will be the same.

### :mahjong:My Code
```js
const charIndex = (word, char) =>
word.includes(char) ?  [word.indexOf(char), word.lastIndexOf(char)]: undefined;
```

## Transforming Words into Binary Strings
Write a function that transforms all letters from [a,m] to 0 and letters from [n,z] to 1 in a string.
```js
Examples
convertBinary("house") ➞ "01110"

convertBinary("excLAIM") ➞ "0100000"

convertBinary("moon") ➞ "0111"
```
### :video_game:My Code
```js
const convertBinary = str =>
str.replace(/[a-m]/gi, 0).replace(/[n-z]/gi, 1);
```
## Recursion: Length of a String
Write a function that returns the length of a string. Make your function recursive.
```
Examples
length("apple") ➞ 5

length("make") ➞ 4

length("a") ➞ 1

length("") ➞ 0
```
### :clapper:My Code
```js
const length = str => str === '' ? 0 : 1 + length(str.substring(1));
```

## Sum of Cubes
Create a function that takes in an array of numbers and returns the sum of its cubes.
```js
Examples
sumOfCubes([1, 5, 9]) ➞ 855
// Since 1^3 + 5^3 + 9^3 = 1 + 125 + 729 = 855

sumOfCubes([3, 4, 5]) ➞ 216

sumOfCubes([2]) ➞ 8

sumOfCubes([]) ➞ 0
```
### :hammer:My Code
```js
const sumOfCubes = nums => nums.map(n => Math.pow(n,3))
.reduce((a,b)=> a+b, 0);
```

## Recursion: Factorials
Write a function that calculates the factorial of a number recursively.
```js
Examples
factorial(5) ➞ 120

factorial(3) ➞ 6

factorial(1) ➞ 1

factorial(0) ➞ 1
```
### :smoking:My Code
```js
const factorial = n => n == 0 ? 1 : n * factorial(n-1);
```

## Filter out Strings from an Array
Create a function that takes an array of non-negative numbers and strings and return a new array without the strings.
```
Examples
filterArray([1, 2, "a", "b"]) ➞ [1, 2]

filterArray([1, "a", "b", 0, 15]) ➞ [1, 0, 15]

filterArray([1, 2, "aasf", "1", "123", 123]) ➞ [1, 2, 123]
```
### :bomb:My Code
```js
const filterArray = arr => arr.filter(x => Number.isInteger(x));
```
