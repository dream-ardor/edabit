## Who's The Oldest?
Given an object containing the names and ages of a group of people, return the name of the oldest person.
```js
Examples
oldest({
  Emma: 71,
  Jack: 45,
  Amy: 15,
  Ben: 29
}) ➞ "Emma"

oldest({
  Max: 9,
  Josh: 13,
  Sam: 48,
  Anne: 33
}) ➞ "Sam"
```
### :hamburger:My Code
```js
let oldest = people => Object.keys(people).reduce((a,b)=> people[a] > people[b] ? a : b);
```

## Remove Every Vowel from a String
Create a function that takes a string and returns a new string with all vowels removed.
```js
Examples
removeVowels("I have never seen a thin person drinking Diet Coke.")
➞ " hv nvr sn  thn prsn drnkng Dt Ck."

removeVowels("We're gonna build a wall!")
➞ "W'r gnn bld  wll!"

removeVowels("Happy Thanksgiving to all--even the haters and losers!")
➞ "Hppy Thnksgvng t ll--vn th htrs nd lsrs!"
```
### :fries:My Code
```js
const removeVowels = str => str.replace(/[aeiou]/gi, '');
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
### :meat_on_bone:My Code
```js
const testJackpot = result => result.every((v,a,i)=> v === i[0]);
```

## Sort Numbers in Ascending Order
Create a function that takes an array of numbers and returns a new array, sorted in ascending order (smallest to biggest).

Sort numbers array in ascending order.
If functions argument is null, an empty array or undefined, return an empty array.
Return new array of sorted numbers.
```js
Examples
sortNumsAscending([1, 2, 10, 50, 5]) ➞ [1, 2, 5, 10, 50]

sortNumsAscending([80, 29, 4, -95, -24, 85]) ➞ [-95, -24, 4, 29, 80, 85]

sortNumsAscending(null) ➞ []

sortNumsAscending([]) ➞ []
```
Notes
The numbers being passed to sortNumsAscending() can be positive or negative.
### :apple:My Code
```js
sortNumsAscending = arr => arr == null ? [] :arr.sort((a,b)=> a-b);
```
