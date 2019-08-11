## The Museum of Incredibly Dull Things
A museum wants to get rid of some exhibitions. Vanya, the interior architect, comes up with a plan to remove the most boring exhibitions. She gives them a rating, and removes the one with the lowest rating. Just as she finishes rating the exhibitions, she's called off to an important meeting. She asks you to write a program that tells her the ratings of the items after the lowest one is removed.

Create a function that takes an array of integers and removes the smallest value.
```js
Examples
removeSmallest([1, 2, 3, 4, 5] ) ➞ [2, 3, 4, 5]

removeSmallest([5, 3, 2, 1, 4]) ➞ [5, 3, 2, 4]

removeSmallest([2, 2, 1, 2, 1]) ➞ [2, 2, 2, 1]
```
### :tram:My Code
```js
const removeSmallest = arr => 
(arr.splice(arr.indexOf(Math.min(...arr)),1),arr);
```

## Three Programmers Problem
You hired three programmers and you (hopefully) pay them. Create a function that takes three numbers (the hourly wage of each programmer) and returns the difference between the highest-paid programmer and the lowest-paid.
```js
Examples
programmers(147, 33, 526) ➞ 493

programmers(33, 72, 74) ➞ 41

programmers(1, 5, 9) ➞ 8
```
### :tram:My Code
```js
const programmers = (o, t, th) => Math.max(o,t,th) - Math.min(o,t,th);
```

## Snail Race
Steve and Maurice are racing snails. They each have 3, a slow (s), medium (m) and fast (f) one. Although Steve's snails are all a bit stronger than Maurice's, Maurice has a trick up his sleeve. His plan is (written [Maurice, Steve]):
```
Round 1: [s, f] Sacrifice his slowest snail against Steve's fastest.
Round 2: [m, s] Use his middle snail against Steve's slowest.
Round 3: [f, m] Use his fastest snail against Steve's middle.
```
Create a function that determines whether Maurice's plan will work by outputting true if Maurice wins 2/3 games.

The function inputs:

Array 1: [s, m, f] for Maurice.
Array 2: [s, m, f] for Steve.
```js
Examples
mauriceWins([3, 5, 10], [4, 7, 11]) ➞ true
// Since the matches are (3, 11), (5, 4) and (10, 7), Maurice wins 2 out of 3.

mauriceWins([6, 8, 9], [7, 12, 14]) ➞ false
// Since the matches are (6, 14), (8, 7) and (9, 12), Steve wins 2 out of 3.

mauriceWins([1, 8, 20], [2, 9, 100]) ➞ true
```
### :tram:My Code
```js
const mauriceWins = (m, s) => m[1] > s[0] && m[2] > s[1];
```

## Convert to Hex
Create a function that takes a strings characters as ASCII and returns each characters hexadecimal value as a string.
```js
Examples
toHex("hello world") ➞ "68 65 6c 6c 6f 20 77 6f 72 6c 64"

toHex("Big Boi") ➞ "42 69 67 20 42 6f 69"

toHex("Marty Poppinson") ➞ "4d 61 72 74 79 20 50 6f 70 70 69 6e 73 6f 6e"
```
```
Notes
Each byte must be seperated by a space.
All alpha hex characters must be lowercase.
```
### :tram:My Code
```js
const toHex = str =>
str.split('').map(x => x.charCodeAt(0).toString(16)).join(' ');

//using for loop
function toHex(str) {
  let arr = [];
  for(i = 0, l = str.length; i < l; i++) {
  let hex = Number(str.charCodeAt(i)).toString(16);
   arr.push(hex);
  }
   return arr.join(' ');
}
```

## Return the Index of All Capital Letters
Create a function that takes a single string as argument and returns an ordered list containing the indexes of all capital letters in the string.
```js
Examples
indexOfCaps("eDaBiT") ➞ [1, 3, 5]

indexOfCaps("eQuINoX") ➞ [1, 3, 4, 6]

indexOfCaps("determine") ➞ []

indexOfCaps("STRIKE") ➞ [0, 1, 2, 3, 4, 5]

indexOfCaps("sUn") ➞ [1]
```
```
Notes
Return an empty array if no uppercase letters are found in the string.
Special characters ($#@%) and numbers will be included in some test cases.
```
### :tram:My Code
```js
const indexOfCaps = str => {
  let caps = [];
  for(i = 0; i < str.length; i++) {
   if(str[i].match(/[A-Z]/) != null){
   caps.push(i);
   }
 }
  return caps;
}
```
