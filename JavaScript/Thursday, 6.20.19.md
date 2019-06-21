## Return the First and Last Elements in an Array :loop:
Create a function that takes an array of numbers and return the first and last elements as a new array.
```js
Examples
firstLast([5, 10, 15, 20, 25]) ➞ [5, 25]

firstLast(["edabit", 13, null, false, true]) ➞ ["edabit", true]

firstLast([undefined, 4, "6", "hello", null]) ➞ [undefined, null]
```

### My Code
```js
const firstLast = arr => [arr[0], arr[arr.length -1]];
```

## Get Word Count :mag:
Create a function that takes a string and returns the word count. The string will be a sentence.
```js
Examples
countWords("Just an example here move along") ➞ 6

countWords("This is a test") ➞ 4

countWords("What an easy task, right") ➞ 5
```
### My Code
```js
const countWords = str => str.split(" ").length;
```

## Exists a Number Higher? :mag_right:
Write a function that returns true if there exists at least one number that is larger than or equal to n.
```js
Examples
existsHigher([5, 3, 15, 22, 4], 10) ➞ true

existsHigher([1, 2, 3, 4, 5], 8) ➞ false

existsHigher([4, 3, 3, 3, 2, 2, 2], 4) ➞ true

existsHigher([], 5) ➞ false
```
### My Code
```js
const existsHigher = (arr, n) => Math.max(...arr) >= n ? true : false;
```
