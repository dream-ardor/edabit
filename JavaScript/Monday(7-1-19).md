## Minimum Removals to Make Sum Even
Create a function that returns the minimum number of removals to make the sum of all elements in an array even.
```js
Examples
minimumRemovals([1, 2, 3, 4, 5]) ➞ 1

minimumRemovals([5, 7, 9, 11]) ➞ 0

minimumRemovals([5, 7, 9, 12]) ➞ 1
```
### :basketball:My Code 
```js
const minimumRemovals = arr => arr.reduce((a,b)=> a+b) % 2 ? 1 : 0;
```
## Filter out Strings from a List
Create a function which filters out strings from an array and returns a new array containing only integers.
```js
Examples
filterList([1, 2, 3, "x", "y", 10]) ➞ [1, 2, 3, 10]

filterList([1, "a", 2, "b", 3, "c"]) ➞ [1, 2, 3]

filterList([0, -32, "&@A", 64, "99", -128]) ➞ [0, -32, 64, -128]
```
### :soccer:My Code
```js
const filterList = l => l.filter(item =>
(typeof item === "number"));
```

## Return the Four Letter Strings
Create a function that takes an array of strings. Return all words in the array that are exactly four letters.
```js
Examples
isFourLetters(["Ryan", "Kieran", "Jason", "Matt"]) ➞ ["Ryan", "Matt"]

isFourLetters(["Tomato", "Potato", "Pair"]) ➞ ["Pair"]

isFourLetters(["Kangaroo", "Bear", "Fox"]) ➞ ["Bear"]
```
### :football:My Code
```js
const isFourLetters = arr => arr.filter(x => x.length === 4);
```

## Same Number of Unique Elements
Write a function that returns true if two arrays have the same number of unique elements, and false otherwise.
```js
Examples
same([1, 3, 4, 4, 4], [2, 5, 7]) ➞ true

same([9, 8, 7, 6], [4, 4, 3, 1]) ➞ false

same([2], [3, 3, 3, 3, 3]) ➞ true
```
### :tennis:My Code
```js
const same = (a1, a2) => new Set(a1).size === new Set(a2).size;
```

## Eliminate Odd Numbers within an Array
Create a function that takes an array of numbers and returns only the even values.
```js
Examples
noOdds([1, 2, 3, 4, 5, 6, 7, 8]) ➞ [2, 4, 6, 8]

noOdds([43, 65, 23, 89, 53, 9, 6]) ➞ [6]

noOdds([718, 991, 449, 644, 380, 440]) ➞ [718, 644, 380, 440]
```
### :baseball:My Code
```js
const noOdds = arr => arr.filter(x => x % 2 === 0);
```

## Repeat the Same Item Multiple Times
Create a function that takes two arguments (item, times). The first argument (item) is the item that needs repeating while the second argument (times) is the number of times the item is to be repeated. Return the result in an array.
```js
Examples
repeat("edabit", 3) ➞ ["edabit", "edabit", "edabit"]

repeat(13, 5) ➞ [13, 13, 13, 13, 13]

repeat("7", 2) ➞ ["7", "7"]

repeat(0, 0) ➞ []
```
### :8ball:My Code
```js
const repeat = (item, times) => Array(times).fill(item);
```
## State Names and Abbreviations
Create a function that filters out an array of state names into two categories based on the second parameter.
```js
Abbreviations abb
Full names full
Examples
filterStateNames(["Arizona", "CA", "NY", "Nevada"], "abb")
➞ ["CA", "NY"]

filterStateNames(["Arizona", "CA", "NY", "Nevada"], "full")
➞ ["Arizona", "Nevada"]

filterStateNames(["MT", "NJ", "TX", "ID", "IL"], "abb")
➞ ["MT", "NJ", "TX", "ID", "IL"]

filterStateNames(["MT", "NJ", "TX", "ID", "IL"], "full")
➞ []
```
### :golf: My Code
```js
const filterStateNames = (arr, type) => type === "abb" ?
arr.filter(x => x.length === 2) : arr.filter(x => x.length > 2;)
```
## Alphabet Soup
Create a function that takes a string and returns a string with its letters in alphabetical order.
```js
Examples
AlphabetSoup("hello") ➞ "ehllo"

AlphabetSoup("edabit") ➞ "abdeit"

AlphabetSoup("hacker") ➞ "acehkr"

AlphabetSoup("geek") ➞ "eegk"

AlphabetSoup("javascript") ➞ "aacijprstv"
```
### :bowling: My Code
```js
const AlphabetSoup = str => str.split('').sort().join('');
```

