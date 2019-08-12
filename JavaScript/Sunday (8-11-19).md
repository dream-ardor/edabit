## Flash Cards
Create a function that outputs the results of a flashcard. A flashcard is an array of three elements: a number, an operator symbol, and another number. Return the mathematical result of that expression.

There are 4 operators: + (addition), - (subtraction), x (multiplication), and / (division). If the flashcard displays a number being divided by zero, e.g. [3, "/", 0], then return undefined. For division, round to the hundredths place. So [10, "/", 3] should return 3.33.
```js
Examples
flash([3, "x", 7]) ➞ 21

flash([5, "+", 7]) ➞ 12

flash([10, "-", 9]) ➞ 1

flash([10, "/", 0]) ➞ undefined

flash([10, "/", 3]) ➞ 3.33
```
### My Code
```js
const flash = ([num1, op, num2]) =>
op === '/' && num2 === 0 ? undefined :
op === 'x' ? num1 * num2 :
op === '-' ? num1 - num2 :
op === '+' ? num1 + num2 :
op === '/' ? +(num1 / num2).toFixed(2) : 0;
```

## Positive Count / Negative Sum
Create a function that takes an array of positive and negative numbers. Return an array where the first element is the count of positive numbers and the second element is the sum of negative numbers.
```js
Examples
countPosSumNeg([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, -11, -12, -13, -14, -15]) ➞ [10, -65]

countPosSumNeg([92, 6, 73, -77, 81, -90, 99, 8, -85, 34]) ➞ [7, -252]

countPosSumNeg([91, -4, 80, -73, -28]) ➞ [2, -105]

countPosSumNeg(null) ➞ []

countPosSumNeg([]) ➞ []
```
### My Code
```js
function countPosSumNeg(arr) {
  if (!arr || !arr.length)return [];
 let a = arr.filter(x => x > 0);
 let b = arr.filter(x => x < 0);
  return [a.length, b.reduce((a,b)=> a+b, 0)];
}
```

## Volume of a Cone
Create a function that takes the height and radius of a cone as arguments and returns the volume of the cone. See the resources tab for the formula.
```js
Examples
coneVolume(3, 2) ➞ 12.57

coneVolume(15, 6) ➞ 565.49

coneVolume(18, 0) ➞ 0
```
### My Code
```js
const coneVolume = (h, r) => +((1/3) * Math.PI * Math.pow(r,2) * h).toFixed(2);
```

## Days in a Month
Create a function that takes the month and year (as integers) and returns the number of days in that month.
```js
Examples
days(2, 2018) ➞ 28

days(3, 2011) ➞ 31

days(4, 654) ➞ 30

days(2, 2020) ➞ 29

days(2, 200) ➞ 28

days(2, 1000) ➞ 29
```

## My Code
```js
const days = (month, year) =>
  new Date(year, month, 0).getDate();
```


