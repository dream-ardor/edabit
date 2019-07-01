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
### :cd: My Code 
```js
let sumOfCubes = nums => nums.map(x => Math.pow(x ,3))
.reduce((a,b)=> a+b,0); 
```

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
If the character does not exist in the word, return undefined.
If only one instance of the character exists, the first and last index will be the same.
Check the Resources tab for hints.

### :dvd: My Code
```js
const charIndex = (word, char) => word.includes(char) ?
[word.indexOf(char),word.lastIndexOf(char)] : undefined;

```

## Repeating Letters
Create a function that takes a string and returns a string in which each character is repeated once.
```js
Examples
doubleChar("String") ➞ "SSttrriinngg"

doubleChar("Hello World!") ➞ "HHeelllloo  WWoorrlldd!!"

doubleChar("1234!_ ") ➞ "11223344!!__  "
```
### :camera: My Code
```js
const doubleChar = str => str.split('').map(x => x + x).join('');
```

## X and Y Coordinates
Create a function that converts two arrays of x- and y- coordinates into an array of (x,y) coordinates.
```js
Examples
convertCartesian([1, 5, 3, 3, 4], [5, 8, 9, 1, 0])
➞ [[1, 5], [5, 8], [3, 9], [3, 1], [4, 0]]

convertCartesian([9, 8, 3], [1, 1, 1])
➞ [[9, 1], [8, 1], [3, 1]]
```
### :tv: My Code
```js
const convertCartesian = (x, y) => x.map((x,z) => [x, y[z]]); 
```

## Say "Hello" Say "Bye"
Write a function that takes a string name and a number num (either 0 or 1) and return "Hello" + name if num is 1, otherwise return "Bye" + name.
```js
Examples
sayHelloBye("alon", 1) ➞ "Hello Alon"

sayHelloBye("Tomi", 0) ➞ "Bye Tomi"

sayHelloBye("jose", 0) ➞ "Bye Jose"
```
### :video_camera:My Code
```js
const sayHelloBye = (name, num) => num === 1 ? "Hello " + name.charAt(0).toUpperCase() + name.slice(1)
: "Bye " + name.charAt(0).toUpperCase() + name.slice(1);
```

