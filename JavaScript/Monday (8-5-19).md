## Primes Below a Given Number
Create a function that will find all primes below a given number. Return the result as an array.
```js
Examples
primesBelowNum(5) ➞ [2, 3, 5]

primesBelowNum(10) ➞ [2, 3, 5, 7]

primesBelowNum(20) ➞ [2, 3, 5, 7, 11, 13, 17, 19]
```
### :stars:My Code
```js
function primesBelowNum(n) {
  let arr = [2];
   for (i = 3; i <= n; i += 2) {
     if (arr.every(a => i % a != 0)) {
       arr.push(i)
     }
  }
   return arr;
}
```

## Fix The Spacing
Additional spaces have been added to a sentence. Return the correct sentence by removing them. All words should be separated by one space, and there should be no spaces at the beginning or end of the sentence.
```js
Examples
correctSpacing("The film   starts       at      midnight. ")
➞ "The film starts at midnight."

correctSpacing("The     waves were crashing  on the     shore.   ")
➞ "The waves were crashing on the shore."

correctSpacing(" Always look on    the bright   side of  life.")
➞ "Always look on the bright side of life."
```
### :stars:My Code
```js
const correctSpacing = sentence => sentence.replace(/\s+/g,' ').trim();
```
## ASCII Charts (Part 1: Progress Bar)
Given a character and a value between 0 and 100, return a string that represents a simple progress bar.
```
The value represents a percentage.
The bar should begin and end with "|"
Repeat the character to fill the bar, with each character equivalent to 10%
Use spaces to pad the bar to a length of 10 characters.
A single space comes after the bar, then a message with the % completion (e.g. "Progress: 60%")
If the value is 100, the message should be "Completed!".
```
```js
Examples
progressBar("#", 0)   ➞ "|          | Progress: 0%"

progressBar("=", 40)  ➞ "|====      | Progress: 40%"

progressBar("#", 60)  ➞ "|######    | Progress: 60%"

progressBar(">", 100) ➞ "|>>>>>>>>>>| Completed!"
```
### :stars:My Code
```js
function progressBar(bar, progress) {
 return "|" + bar.repeat(progress/10) + ' '.repeat(10 - (progress/10))
+ "| " + (progress === 100 ? "Completed!" : "Progress: " + progress + "%")
}

```

## GCD and LCM ( Part 1)
Create a function that takes two numbers as arguments and returns the GCD of the two numbers.
```js
Examples
gcd(3, 5) ➞ 1

gcd(14, 28) ➞ 14

gcd(4, 18) ➞ 2
```
### :stars:My Code
```js
const gcd = (a, b) => !b ? a : gcd(b, a % b)
```
## Halve and Halve Again
Given two integers a and b, return how many times a can be halved while still being greater than b.
```js
Examples
halveCount(1324, 98) ➞ 3
// (1324 -> 662 -> 331 -> 165.5)

halveCount(624, 8) ➞ 6
// (624 -> 312 -> 156 -> 78 -> 39 -> 19.5 -> 9.75)

halveCount(1000, 3) ➞ 8
// (1000 -> 500 -> 250 -> 125 -> 62.5 -> 31.25 -> 15.625 -> 7.8125 -> 3.90625)
```
### :stars:My Code
```js
function halveCount(a, b) {
  let a1 = 0;
  while(a/2 > b) {
   a = a/2;
   a1++;
  }
  return a1;
}
```
## Upper or Lower Case
Return the smallest number of steps it takes to convert a string entirely into uppercase or entirely into lower case, whichever takes the fewest number of steps. A step consists of changing one character from lower to upper case, or vice versa.
```js
Examples
stepsToConvert("abC") ➞ 1
// "abC" converted to "abc" in 1 step

stepsToConvert("abCBA") ➞ 2
// "abCBA" converted to "ABCBA" in 2 steps

stepsToConvert("aba") ➞ 0

stepsToConvert("abaCCC") ➞ 3
```
### :stars:My Code
```js
const stepsToConvert = str => {
  let a = [...str].filter(x => x === x.toUpperCase());
  let b = [...str].filter(x => x === x.toLowerCase());
 return Math.min(a.length, b.length);
}

//using some regex
function stepsToConvert(str) {
  if(str == '') { return 0}
  if(str == str.toUpperCase() || str == str.toLowerCase()){return 0}
  let a = str.match(/[a-z]/g).length;
  let b = str.match(/[A-Z]/g).length;
  return Math.min(a,b);
}
```






