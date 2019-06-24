## Remove the First and Last Characters

Create a function that removes the first and last characters from a string.
```js
Examples
removeFirstLast("hello") ➞ "ell"

removeFirstLast("maybe") ➞ "ayb"

removeFirstLast("benefit") ➞ "enefi"

removeFirstLast("a") ➞ "a"
```

## My Code :flashlight:
```js
const removeFirstLast = str => str.length > 2 ? 
str.slice(1, -1) : str;
```

## Little Dictionary
Create a function that takes in an initial word and filters out an array to contain words that start with the same letters as the initial word.
```js
Examples
dictionary("bu", ["button", "breakfast", "border"]) ➞ ["button"]

dictionary("tri", ["triplet", "tries", "trip", "piano", "tree"]) ➞ ["triplet", "tries", trip"]

dictionary("beau", ["pastry", "delicious", "name", "boring"]) ➞ []
```
## My Code :email:
```js
const dictionary = (initial, words) =>
words.filter(x => x.startsWith(initial));
```

## Repeating Letters N Times
Create a function that repeats each character in a string n times.
```js
Examples
repeat("mice", 5) ➞ "mmmmmiiiiiccccceeeee"

repeat("hello", 3) ➞ "hhheeellllllooo"

repeat("stop", 1) ➞ "stop"
```
## My Code :calling:
```js
const repeat=(str, n) => {
let x = str.split('').map(x => x.repeat(n));
return x.join('');
}

```

## Hurdle Jump
Create a function that takes an array of hurdle heights and a jumper's jump height, and determine whether or not the hurdler can clear all the hurdles.

A hurdler can clear a hurdle if their jump height is greater than or equal to the hurdle height.
```js
Examples
hurdleJump([1, 2, 3, 4, 5], 5) ➞ true

hurdleJump([5, 5, 3, 4, 5], 3) ➞ false

hurdleJump([5, 4, 5, 6], 10) ➞ true

hurdleJump([1, 2, 1], 1) ➞ false
```
## My Code :running:
```js
const hurdleJump = (hurdles, jumpHeight) => 
hurdles.every(x => x <= jumpHeight) ? true : false;
```

## Get Student Names
Create a function that takes an array of students and returns an array of student names.
```js
Examples
getStudentNames([
  { name: "Steve" },
  { name: "Mike" },
  { name: "John" }
]) ➞ ["Steve", "Mike", "John"]
```
## My Code :point_down:
```js
const getStudentNames = students => students.map(x => x.name)
```







