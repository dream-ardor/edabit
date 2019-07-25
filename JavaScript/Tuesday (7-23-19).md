## Factorize a Number
Create a function that takes a number as its argument and returns an array of all its factors.
```js
Examples
factorize(12) ➞ [1, 2, 3, 4, 6, 12]

factorize(4) ➞ [1, 2, 4]

factorize(17) ➞ [1, 17]
```
### :secret:My Code
```js
const factorize = num => Array.from(Array(num+1),(_,i)=> i).filter(i=>num % i === 0)
```

## Compare by ASCII Codes
Create a function to that compares two words based on the sum of their ASCII codes and returns the word with the smaller ASCII sum.
```js
Examples
asciiSort(["hey", "man"]) ➞ "man"
// ["h", "e", "y"] ➞ sum([104, 101, 121]) ➞ 326
// ["m", "a", "n"] ➞ sum([109, 97, 110]) ➞ 316

asciiSort(["majorly", "then"]) ➞ "then"

asciiSort(["victory", "careless"]) ➞ "victory"
```
### :sunny:My Code
```js
const asciiSort = arr => {
	let a = arr[0].split('').map(x=>x.charCodeAt()).reduce((a,b)=>a+b);
	let b = arr[1].split('').map(x=>x.charCodeAt()).reduce((a,b)=>a+b);
	 return a < b ? arr[0] : arr[1c]
}
```

## GCD of Two Numbers
Write a function that returns the greatest common divisor (GCD) of two integers.
```js
Examples
gcd(32, 8) ➞ 8

gcd(8, 12) ➞ 4

gcd(17, 13) ➞ 1
```

### :cyclone:My Code
```js
const gcd = (a,b) => !b ? a : gcd(b, a % b);
```

## AlTeRnAtInG CaPs
Create a function that alternates the case of the characters in a string.
In the final string, the case should be opposite for every adjacent letter.

⚠️If the instructions are unclear check out the tests and the comments, apparently I can't explain this challenge to save my life.
```js
Examples
alternatingCaps("Hello") ➞ "HeLlO"

alternatingCaps("Hey, how are you?") ➞ "HeY, hOw aRe yOu?"

alternatingCaps("OMG!!! This website is awesome!!") ➞ "OmG!!! tHiS WeBsItE Is aWeSoMe!!"
```
### :foggy:My Code
```js
const alternatingCaps = str => str.split('')
.map((a,b)=> b % 2 === 0 ? a.toUpperCase() : a.toLowerCase())
.join('');

## Equality of 3 Values
Create a function that takes three integer arguments (a, b, c) and returns the number of equal values.
```js
Examples
equal(3, 4, 3) ➞ 2

equal(1, 1, 1) ➞ 3

equal(3, 4, 1) ➞ 0
```
### :ocean:My Code
```js
const equal = (a, b, c) =>
a == b && a == c ? 3 : a == b || b == c || a == c ? 2 : 0;
```
