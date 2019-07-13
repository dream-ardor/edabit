## Factorial of a Positive Integer
Write a function that takes a positive integer and return its factorial.
```js
Examples
factorial(4) ➞ 24

factorial(0) ➞ 1

factorial(9) ➞ 362880
```
Notes
* The factorial of zero is 1.
* The factorial of any positive integer Z is Z * (Z - 1) * (Z - 2) * . . . . . . * 1 (e.g. factorial of 3 is 3 * 2 * 1 = 6)
### :iphone:My Code
```js
const factorial = z => z <= 1 ? 1: z * factorial(z-1);
```

## Scrabble Hand
Given an array of scrabble tiles, create a function that outputs the maximum possible score a player can achieve by summing up the total number of points for all the tiles in their hand. Each hand contains 7 scrabble tiles.

Here's an example hand:
```js
[
  { tile: "N", score: 1 },
  { tile: "K", score: 5 },
  { tile: "Z", score: 10 },
  { tile: "X", score: 8 },
  { tile: "D", score: 2 },
  { tile: "A", score: 1 },
  { tile: "E", score: 1 }
]
```
The players maximumScore from playing all these tiles would be 1 + 5 + 10 + 8 + 2 + 1 + 1, or 28.
```js
Examples
maximumScore([
  { tile: "N", score: 1 },
  { tile: "K", score: 5 },
  { tile: "Z", score: 10 },
  { tile: "X", score: 8 },
  { tile: "D", score: 2 },
  { tile: "A", score: 1 },
  { tile: "E", score: 1 }
]) ➞ 28

maximumScore([
  { tile: "B", score: 2 },
  { tile: "V", score: 4 },
  { tile: "F", score: 4 },
  { tile: "U", score: 1 },
  { tile: "D", score: 2 },
  { tile: "O", score: 1 },
  { tile: "U", score: 1 }
]) ➞ 15
```
### :watch:My Code
```js
const maximumScore = tileHand =>
tileHand.reduce((x,y)=> x + y.score, 0);
```

## "EdaBit" Challenge
Create a function that returns the array of numbers from a given range. But for multiples of three, return “Eda” instead of the number and for the multiples of five, return “Bit”. For numbers which are multiples of both three and five, return “EdaBit”.
```js
Examples
edaBit(0, 10) ➞ [0, 1, 2, "Eda", 4, "Bit", "Eda", 7, 8, "Eda", "Bit" ]

edaBit(14, 20) ➞ [14,  "EdaBit", 16, 17,  "Eda", 19, "Bit" ]

edaBit(99, 106) ➞ ["Eda", "Bit", 101, "Eda", 103, 104, "EdaBit", 106 ]
Notes
In case the number 0 happens to be in the range, return "EdaBit" as well.
```
### :computer:My Code
```js
const edaBit = (start, end) => Array(end - start + 1).fill().map((_,idx)=> start + idx)
.map(x => x % 3===0 && x % 5===0 ? "EdaBit": x % 3 === 0 ? "Eda" : x % 5===0 ? "Bit": x == 0 ? "EdaBit" : x);
```

## Index Shuffle
Create a function takes all even-indexed characters and odd-indexed characters from a string and concatenates them together.

To illustrate:
```js
indexShuffle("abcd") ➞ "acbd"
// "ac" (even-indexed) + "bd" (odd-indexed)
Examples
indexShuffle("abcdefg") ➞ "acegbdf"

indexShuffle("holiday") ➞ "hldyoia"

indexShuffle("maybe") ➞ "myeab"
```
### :vhs:My Code
```js
const indexShuffle = str => str.split('')
.filter((b,c)=>c%2===0).join('')
.concat(str.split('').filter((a,i)=>i%2===1).join(''));
```

## Count Ones in a 2D Array
Create a function to count the number of 1s in a 2D array.
```js
Examples
countOnes([
  [1, 0],
  [0, 0]
]) ➞ 1

countOnes([
  [1, 1, 1],
  [0, 0, 1],
  [1, 1, 1]
]) ➞ 7

countOnes([
  [1, 2, 3],
  [0, 2, 1],
  [5, 7, 33]
]) ➞ 2
```
### :electric_plug:My Code
```js
const countOnes = matrix => matrix.join('').replace(/[^1]/g,'').length;

//using reduce
const countOnes = matrix.reduce((a,b)=> a + b.reduce((c,d)=> c + (d==1),0),0);
```

## Absolute Sum
Take an array of integers (positive or negative or both) and return the sum of the absolute value of each element.
```js
Examples
getAbsSum([2, -1, 4, 8, 10]) ➞ 25

getAbsSum([-3, -4, -10, -2, -3]) ➞ 22

getAbsSum([2, 4, 6, 8, 10]) ➞ 30

getAbsSum([-1]) ➞ 1
```
### :flashlight:My Code
```js
const getAbsSum = arr => arr == -1 ? 1 : arr.reduce((a,b)=> Math.abs(a) + Math.abs(b));
```

## Recursion: GCD
Write a function that calculates the GCD (Greatest Common Divisor) of two numbers recursively.
```js
Examples
gcd(10, 20) ➞ 10

gcd(1, 3) ➞ 1

gcd(5, 7) ➞ 1

gcd(2, 6) ➞ 2
```
### My Code
```js
const gcd = (a, b) => !b ? a : gcd(b, a % b);
```

## Calculate the Profit
You work for a manufacturer, and have been asked to calculate the total profit made on the sales of a product. You are given an object containing the cost price per unit (in dollars), sell price per unit (in dollars), and the starting inventory. Return the total profit made, rounded to the nearest dollar. Assume all of the inventory has been sold.
```js
Examples
profit({
  costPrice: 32.67,
  sellPrice: 45.00,
  inventory: 1200
}) ➞ 22650

profit({
  costPrice: 225.89,
  sellPrice: 550.00,
  inventory: 100
}) ➞ 32411

profit({
  costPrice: 2.77,
  sellPrice: 7.95,
  inventory: 8500
}) ➞ 44030
```
### :bulb:My Code
```js
const profit = info => Math.round((info.sellPrice * info.inventory)-
(info.costPrice * info.inventory));
```
