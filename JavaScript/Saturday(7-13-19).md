## Return the Factorial
Create a function that takes an integer and returns the factorial of that integer. That is, the integer multiplied by all positive lower integers.
```js
Examples
factorial(3) ➞ 6

factorial(5) ➞ 120

factorial(13) ➞ 6227020800
```
### :construction:My Code
```js
const factorial = n => n <= 2 ? n : n * factorial(n-1);
```
## Maximum Difference
Given an array of integers, return the difference between the largest and smallest integers in the array.
```js
Examples
difference([10, 15, 20, 2, 10, 6]) ➞ 18
// 20 - 2 = 18

difference([-3, 4, -9, -1, -2, 15]) ➞ 24
// 15 - (-9) = 24
```
### :vertical_traffic_light:My Code
```js
const difference = nums => Math.max(...nums) - Math.min(...nums);
```

## Total Volume
Given an array of boxes, create a function that returns the total volume of all those boxes combined together. A box is represented by an array with three elements: length, width and height.

For instance, totalVolume([2, 3, 2], [6, 6, 7], [1, 2, 1]) should return 266 since (2 x 3 x 2) + (6 x 6 x 7) + (1 x 2 x 1) = 12 + 252 + 2 = 266.
```js
Examples
totalVolume([4, 2, 4], [3, 3, 3], [1, 1, 2], [2, 1, 1]) ➞ 63

totalVolume([2, 2, 2], [2, 1, 1]) ➞ 10

totalVolume([1, 1, 1]) ➞ 1
```

### :traffic_light:My Code
```js
const totalVolume = (...boxes) =>
boxes.reduce((a,b)=> a + b.reduce((c,d)=> c * d, 1), 0);
```

## Is the Number Symmetrical?
Create a function that takes a number as an argument and returns true or false depending on whether the number is symmetrical or not. A number is symmetrical when it is the same as its reverse.
```js
Examples
isSymmetrical(7227) ➞ true

isSymmetrical(12567) ➞ false

isSymmetrical(44444444) ➞ true

isSymmetrical(9939) ➞ false

isSymmetrical(1112111) ➞ true
```
### :checkered_flag:My Code
```js
const isSymmetrical = num => num == num.toString().split('').reverse().join('');
```

## Pi to N Decimal Places
Given a number n, write a function that returns PI to n decimal places.
```js
Examples
myPi(5) ➞ 3.14159

myPi(4) ➞ 3.1416

myPi(15) ➞ 3.141592653589793
```
### :moyai:My Code
```js
const myPi = n => +Math.PI.toFixed(n);
```
## Sort an Array by String Length
Create a function that takes an array of strings and return an array, sorted from shortest to longest.
```
Examples
sortByLength(["Google", "Apple", "Microsoft"])
➞ ["Apple", "Google", "Microsoft"]

sortByLength(["Leonardo", "Michelangelo", "Raphael", "Donatello"])
➞ ["Raphael", "Leonardo", "Donatello", "Michelangelo"]

sortByLength(["Turing", "Einstein", "Jung"])
➞ ["Jung", "Turing", "Einstein"]
```
### :fuelpump:My Code
```js
const sortByLength = arr => arr.sort((a,b) => a.length - b.length);
```
## Fix the Error: Value vs. Reference Types
Create a function that returns true if two arrays contain identical values, and false otherwise.

To solve this question, your friend writes the following code:
```js
function checkEquals(arr1, arr2) {
if (arr1 === arr2) {
  return true
 } else {
  return false
 }
}
```
But testing the code, you see that something is not quite right. Running the code yields the following results:
```js
checkEquals([1, 2], [1, 3]) ➞ false
// Good so far...

checkEquals([1, 2], [1, 2]) ➞ false
// Yikes! What happened?
```
Rewrite your friend's code so that it correctly checks if two arrays are equal. The tests below should pass:
```js
Examples
checkEquals([1, 2], [1, 3]) ➞ false

checkEquals([1, 2], [1, 2]) ➞ true

checkEquals([4, 5, 6], [4, 5, 6]) ➞ true

checkEquals([4, 7, 6], [4, 5, 6]) ➞ false
```
Notes
Hint: This has to do with value vs. reference types.

### :hotsprings:My Code
```js
const checkEquals = (arr1, arr2) => JSON.stringify(arr1) === JSON.stringify(arr2);
```
##Convenience Store
Given a total due and an array representing the amount of change in your pocket, determine whether or not you are able to pay for the item. Change will always be represented in the following order: quarters, dimes, nickels, pennies.

To illustrate: changeEnough([25, 20, 5, 0], 4.25) should yield true, since having 25 quarters, 20 dimes, 5 nickels and 0 pennies gives you 6.25 + 2 + .25 + 0 = 8.50.
```js
Examples
changeEnough([2, 100, 0, 0], 14.11) ➞ false

changeEnough([0, 0, 20, 5], 0.75) ➞ true

changeEnough([30, 40, 20, 5], 12.55) ➞ true

changeEnough([10, 0, 0, 50], 3.85) ➞ false

changeEnough([1, 0, 5, 219], 19.99) ➞ false
```
```
Notes
quarter: 25 cents / $0.25
dime: 10 cents / $0.10
nickel: 5 cents / $0.05
penny: 1 cent / $0.01
```
### :no_smoking:My Code
```js
function changeEnough(change, amountDue) {
  const [q,d,n,p] = change;
	return amountDue <= [(q*.25) + (d*.10) + (n*.05) + (p*.01)];
}
```
