## Is the String in Order?
Create a function that takes a string and returns true or false, depending on whether the characters are in order or not.
```js
Examples
isInOrder("abc") ➞ true

isInOrder("edabit") ➞ false

isInOrder("123") ➞ true

isInOrder("xyzz") ➞ true
```
### :1st_place_medal: My Code
```js
const isInOrder = str => str === str.split('').sort().join('');
```
## Reverse Coding Challenge #6
This is a reverse coding challenge. Normally you're given explicit directions with how to create a function. Here, you must generate your own function to satisfy the relationship between the inputs and outputs.

Your task is to create a function that, when fed the inputs below, produce the sample outputs shown.
```js
Examples
mysteryFunc(152) ➞ 10

mysteryFunc(832) ➞ 48

mysteryFunc(19) ➞ 9

mysteryFunc(133) ➞ 9
```
### :1st_place_medal: My Code
```js
const mysteryFunc = n => 
n.toString().split('').reduce((a,b)=> a * b);
```
## The Museum of Incredibly Dull Things
A museum wants to get rid of some exhibitions. Vanya, the interior architect, comes up with a plan to remove the most boring exhibitions. She gives them a rating, and removes the one with the lowest rating. Just as she finishes rating the exhibitions, she's called off to an important meeting. She asks you to write a program that tells her the ratings of the items after the lowest one is removed.

Create a function that takes an array of integers and removes the smallest value.
```js
Examples
removeSmallest([1, 2, 3, 4, 5] ) ➞ [2, 3, 4, 5]

removeSmallest([5, 3, 2, 1, 4]) ➞ [5, 3, 2, 4]

removeSmallest([2, 2, 1, 2, 1]) ➞ [2, 2, 2, 1]
```
### :1st_place_medal: My Code
```js
const removeSmallest = a => {
  a = a.slice();
  a.splice( a.indexOf(Math.min.apply(null, a)),1)
  return a;
}
```

## Index Multiplier
Return the sum of all items in an array, where each item is multiplied by its index (zero-based). For empty arrays, return 0.
```js
Examples
indexMultiplier([1, 2, 3, 4, 5]) ➞ 40
// (1*0 + 2*1 + 3*2 + 4*3 + 5*4)

indexMultiplier([-3, 0, 8, -6]) ➞ -2
// (-3*0 + 0*1 + 8*2 + -6*3)
```
### :1st_place_medal: My Code
```js
const indexMultiplier = a => a.reduce((a,b,c) => a + (b * c), 0);
```
## A Redundant Function
Write a function redundant that takes in a string str and returns a function that returns str.
```js
Examples
const f1 = redundant("apple")
f1() ➞ "apple"

const f2 = redundant("pear")
f2() ➞ "pear"

const f3 = redundant("")
f2() ➞ ""
```
### :1st_place_medal: My Code
```js
const redundant = s => () => s;

```
## Valid Hex Code
Create a function that determines whether a string is a valid hex code.

A hex code must begin with a pound key # and is exactly 6 characters in length. Each character must be a digit from 0-9 or an alphabetic character from A-F. All alphabetic characters may be uppercase or lowercase.
```js
Examples
isValidHexCode("#CD5C5C") ➞ true

isValidHexCode("#EAECEE") ➞ true

isValidHexCode("#eaecee") ➞ true

isValidHexCode("#CD5C58C") ➞ false
// Length exceeds 6

isValidHexCode("#CD5C5Z") ➞ false
// Not all alphabetic characters in A-F

isValidHexCode("#CD5C&C") ➞ false
// Contains unacceptable character

isValidHexCode("CD5C5C") ➞ false
// Missing #
```
### :1st_place_medal: My Code
```js
const isValidHexCode = s => /^#[\dA-F]{6}$/i.test(s);
```


