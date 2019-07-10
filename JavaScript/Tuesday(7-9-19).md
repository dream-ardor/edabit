## Mirror Array
Given an array, transform that array into a mirror.
```js
Examples
mirror([0, 2, 4, 6]) ➞ [0, 2, 4, 6, 4, 2, 0]

mirror([1, 2, 3, 4, 5]) ➞ [1, 2, 3, 4, 5, 4, 3, 2, 1]

mirror([3, 5, 6, 7, 8]) ➞ [3, 5, 6, 7, 8, 7, 6, 5, 3]
```
### :violin:My Code
```js
const mirror = arr => {
 let a = arr.slice().reverse().slice(1);
 let b = arr.concat(a);
  return b;
}
```

## Total Number of Unique Characters
Given two strings, create a function that returns the total number of unique characters from the combined string.
```js
Examples
countUnique("apple", "play") ➞ 5
// "appleplay" has 5 unique characters:
// "a", "e", "l", "p", "y"

countUnique("sore", "zebra") ➞ 7
// "sorezebra" has 7 unique characters:
// "a", "b", "e", "o", "r", "s", "z"

countUnique("a", "soup") ➞ 5
```
### :space_invader:My Code
```js
const countUnique = (s1, s2) =>
String.prototype.concat(...new Set(s1+s2)).length;

//alternatively
const countUnique = (s1,s1) => new Set(s1+s2).size;
```

## Transform into an Array with No Duplicates
A set is a collection of unique items. A set can be formed from an array from removing all duplicate items.
```js
[1, 3, 3, 5, 5, 5]
// original array

[1, 3, 5]
// original array transformed into a set
Create a function that transforms an array into a set.

Examples
set([1, 3, 3, 5, 5]) ➞ [1, 3, 5]

set([4, 4, 4, 4]) ➞ [4]

set([5, 7, 8, 9, 10, 15]) ➞ [5, 7, 8, 9, 10, 15]
```
Notes
Note: For this question, output an array, not a set. These are two distinctly different data structures in Javascript (although they can be converted from one to the other).

### :video_game:My Code
```js
const set = arr => [...new Set(arr)];
```

## Is it Time for Milk and Cookies?
Christmas Eve is almost upon us, so naturally we need to prepare some milk and cookies for Santa! Create a function that accepts a Date object and returns true if it's Christmas Eve (December 24th) and false otherwise. Keep in mind JavaScript's Date month is 0 based, meaning December is the 11th month while January is 0.
```js
Examples
timeForMilkAndCookies(new Date(2013, 11, 24)) ➞ true

timeForMilkAndCookies(new Date(2013, 0, 23)) ➞ false

timeForMilkAndCookies(new Date(3000, 11, 24)) ➞ true
```
### :game_die:My Code
```js
const timeForMilkAndCookies = date =>
date.getMonth() === 11 && date.getDate() === 24 ? true : false;
```
## Find the Index (Part 1)
Create a function that finds the index of a given item.
```js
Examples
search([1, 5, 3], 5) ➞ 1

search([9, 8, 3], 3) ➞ 2

search([1, 2, 3], 4) ➞ -1
```
### :black_joker:My Code
```js
const search = (arr, item) => arr.indexOf(item);
```



