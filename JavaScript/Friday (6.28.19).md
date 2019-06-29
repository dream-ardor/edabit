## Omnipresent Value
A value is omnipresent if it exists in every subarray inside the main array.

To illustrate:

[[3, 4], [8, 3, 2], [3], [9, 3], [5, 3], [4, 3]]
// 3 exists in every element inside this array, so is omnipresent.
Create a function that determines whether an input value is omnipresent for a given array.
```js
Examples
isOmnipresent([[1, 1], [1, 3], [5, 1], [6, 1]], 1) ➞ true

isOmnipresent([[1, 1], [1, 3], [5, 1], [6, 1]], 6) ➞ false

isOmnipresent([[5], [5], [5], [6, 5]], 5) ➞ true

isOmnipresent([[5], [5], [5], [6, 5]], 6) ➞ false
```
### My Code :strawberry:
```js
const isOmnipresent = (arr, val) => arr.every(x => x.includes(val));
```

## Convert to Decimal Notation
Create a function to convert an array of percentages to their decimal equivalents.
```js
Examples
convertToDecimal(["1%", "2%", "3%"]) ➞ [0.01, 0.02, 0.03]

convertToDecimal(["45%", "32%", "97%", "33%"]) ➞ [0.45, 0.32, 0.97, 0.33]

convertToDecimal(["33%", "98.1%", "56.44%", "100%"]) ➞ [0.33, 0.981, 0.5644, 1]
```
### My Code :peach:
```js
const convertToDecimal = perc => perc.map(x => parseFloat(x) / 100);
```

## Reverse the Case
Given a string, create a function to reverse the case. All lower-cased letters should be upper-cased, and vice versa.
```js
Examples
reverseCase("Happy Birthday") ➞ "hAPPY bIRTHDAY"

reverseCase("MANY THANKS") ➞ "many thanks"

reverseCase("sPoNtAnEoUs") ➞ "SpOnTaNeOuS"
```
### My Code :cherries:
```js
const reverseCase = str => str.split('')
.map(x => x === x.toUpperCase() ? x.toLowerCase() : x.toUpperCase())
.join('');
```

## Typing Game
You're in the midst of creating a typing game.

Create a function that takes in two arrays: the array of user-typed words, and the array of correctly-typed words and outputs an array containing 1s (correctly-typed words) and -1s (incorrectly-typed words).
```js
Inputs:
User-typed Array: ["cat", "blue", "skt", "umbrells", "paddy"]
Correct Array: ["cat", "blue", "sky", "umbrella", "paddy"]

Output: [1, 1, -1, -1, 1]
Examples
correctStream(
  ["it", "is", "find"],
  ["it", "is", "fine"]
) ➞ [1, 1, -1]

correctStream(
  ["april", "showrs", "bring", "may", "flowers"],
  ["april", "showers", "bring", "may", "flowers"]
) ➞ [1, -1, 1, 1, 1]
```
### My Code :eggplant:
```js
const correctStream = (user, correct)=>
user.map(x => correct.includes(x) ? 1 : -1);
```

## Nth Smallest Element
Given an unsorted array, create a function that returns the nth smallest element (the smallest element is the first smallest, the second smallest element is the second smallest, etc).
```js
Examples
nthSmallest([1, 3, 5, 7], 1) ➞ 1

nthSmallest([1, 3, 5, 7], 3) ➞ 5

nthSmallest([1, 3, 5, 7], 5) ➞ null

nthSmallest([7, 3, 5, 1], 2) ➞ 3
```
### My Code :lemon:
```js
const nthSmallest = (arr, n) => n > arr.length ? null :
arr.slice(0).sort()[n-1]; 
```

