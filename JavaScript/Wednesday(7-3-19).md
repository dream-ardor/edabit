## Numbers to Arrays and Vice Versa
Write two functions:
```js
toArray(), which converts a number to an array of its digits.
toNumber(), which converts an array of digits back to its number.
Examples
toArray(235) ➞ [2, 3, 5]

toArray(0) ➞ [0]

toNumber([2, 3, 5]) ➞ 235

toNumber([0]) ➞ 0
```
### :school_satchel:My Code
```js
const toArray = num => Array.from(String(num), Number);

const toNumber = arr => +arr.join('');
```

## Retrieve the Last N Elements
Write a function that retrieves the last n elements from an array.
```js
Examples
last([1, 2, 3, 4, 5], 1) ➞ [5]

last([4, 3, 9, 9, 7, 6], 3) ➞ [9, 7, 6]

last([1, 2, 3, 4, 5], 7) ➞ "invalid"

last([1, 2, 3, 4, 5], 0) ➞ []
```
Notes
Return invalid if n exceeds the length of the array.
Return an empty array if n == 0.
### :bell:My Code
```js
const last = (a, n) => n == 0 ? [] : 
n > a.length ? "invalid" : a.slice(-n);
```

## Edaaaaabit
Write a function that takes an integer and returns a string with the given number of "a"s in Edabit.
```
Examples
howManyTimes(5) ➞ "Edaaaaabit"

howManyTimes(0) ➞ "Edbit"

howManyTimes(12) ➞ "Edaaaaaaaaaaaabit"
```
### :minidisc:My Code
```js
const howManyTimes = num => "Ed" + "a".repeat(num) + "bit";
```
## Convert to Decimal Notation
Create a function to convert an array of percentages to their decimal equivalents.
```js
Examples
convertToDecimal(["1%", "2%", "3%"]) ➞ [0.01, 0.02, 0.03]

convertToDecimal(["45%", "32%", "97%", "33%"]) ➞ [0.45, 0.32, 0.97, 0.33]

convertToDecimal(["33%", "98.1%", "56.44%", "100%"]) ➞ [0.33, 0.981, 0.5644, 1]
```
### :phone:My Code
```js
const convertToDecimal = perc => perc.map(x => parseFloat(x)/100);
```

## Find the Smallest and Biggest Numbers
Create a function that takes an array of numbers and return both the minimum and maximum numbers, in that order.
```js
Examples
minMax([1, 2, 3, 4, 5]) ➞ [1, 5]

minMax([2334454, 5]) ➞ [5, 2334454]

minMax([1]) ➞ [1, 1]
```
### :fax:My Code
```js
let minMax = arr => [Math.min(...arr), Math.max(...arr)];
```

## Hashes and Pluses
Create a function that returns the number of hashes and pluses in a string.
```js
Examples
hashPlusCount("###+") ➞ [3, 1]

hashPlusCount("##+++#") ➞ [3, 3]

hashPlusCount("#+++#+#++#") ➞ [4, 6]

hashPlusCount("") ➞ [0, 0]
Notes
It should return [0, 0] for an empty string.
```
### :pager:My Code
```js
const hashPlusCount = str =>
[(str.match(/#/g)|| "").length,
(str.match(/\+/g)|| "").length];
```
## Largest Swap
Write a function that takes a two-digit number and determines if it's the largest of two possible digit swaps.

To illustrate:

largestSwap(27) ➞ false

largestSwap(43) ➞ true
If 27 is our input, we should return false because swapping the digits gives us 72, and 72 > 27. On the other hand, swapping 43 gives us 34, and 43 > 34.
```js
Examples
largestSwap(14) ➞ false

largestSwap(53) ➞ true

largestSwap(99) ➞ true
```
### :sound:My Code
```js
let largestSwap = num => num >=
num.toString().split('').reverse().join('');
```
## Say "Hello" Say "Bye"
Write a function that takes a string name and a number num (either 0 or 1) and return "Hello" + name if num is 1, otherwise return "Bye" + name.
```js
Examples
sayHelloBye("alon", 1) ➞ "Hello Alon"

sayHelloBye("Tomi", 0) ➞ "Bye Tomi"

sayHelloBye("jose", 0) ➞ "Bye Jose"
```
### :mute:My Code
```js
let sayHelloBye = (name, num) => num === 1 ? 
"Hello " + name.charAt(0).toUpperCase()+ name.slice(1) 
:"Bye " + name.charAt(0).toUpperCase()+ name.slice(1);
```
## Reverse the Case
Given a string, create a function to reverse the case. All lower-cased letters should be upper-cased, and vice versa.
```js
Examples
reverseCase("Happy Birthday") ➞ "hAPPY bIRTHDAY"

reverseCase("MANY THANKS") ➞ "many thanks"

reverseCase("sPoNtAnEoUs") ➞ "SpOnTaNeOuS"
```
### :loudspeaker:My Code
```js
const reverseCase = str => str.split('')
.map(x=> x === x.toUpperCase() ? x.toLowerCase() : x.toUpperCase())
.join('');
```
