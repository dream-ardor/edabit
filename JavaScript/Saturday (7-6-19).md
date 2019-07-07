## Move Capital Letters to the Front
Create a function that moves all capital letters to the front of a word.
```js
Examples
capToFront("hApPy") ➞ "APhpy"

capToFront("moveMENT") ➞ "MENTmove"

capToFront("shOrtCAKE") ➞ "OCAKEshrt"
```

## :e-mail:My Code
```js
const capToFront = s =>
s.replace(/[a-z]/g, '') + s.replace(/[A-Z]/g, '')

```

## Find the Index (Part 1)
Create a function that finds the index of a given item.
```js
Examples
search([1, 5, 3], 5) ➞ 1

search([9, 8, 3], 3) ➞ 2

search([1, 2, 3], 4) ➞ -1
```

### :inbox_tray:My Code
```js
const search = (arr, i) => i > arr ? -1 : arr.indexOf(i);
```

## Recursion: Factorials
Write a function that calculates the factorial of a number recursively.
```js
Examples
factorial(5) ➞ 120

factorial(3) ➞ 6

factorial(1) ➞ 1

factorial(0) ➞ 1
```
### :calling:My Code
```js
const factorial = n => n === 0 ? 1 : n * factorial(n- 1);
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
### :moneybag:My Code
```js
const gcd = (a, b) => b != 0 ? gcd(b,(a % b)) : a;
```

## Recursion: Length of a String
Write a function that returns the length of a strength. Make your function recursive.
```js
Examples
length("apple") ➞ 5

length("make") ➞ 4

length("a") ➞ 1

length("") ➞ 0
```
### :dollar:My Code
```js
const length = str => str == '' ? 0 : length(str.substring(1)) + 1
```
## Join Two Portions of a Path
Write a function that receives two portions of a path and joins them. The portions will be joined with the "/" separator. There could be only one separator and if it is not present it should be added.
```js
Examples
joinPath("portion1", "portion2") ➞ "portion1/portion2"

joinPath("portion1/", "portion2") ➞ "portion1/portion2"

joinPath("portion1", "/portion2") ➞ "portion1/portion2"

joinPath("portion1/", "/portion2") ➞ "portion1/portion2"
```
### :gun:My Code
```js
const joinPath = (portion1, portion2) => 
portion1.replace(/\//, '') + "/" + portion2.replace(/\//, '');
```

## Find the Index (Part 2)
Create a function that finds the index of a given item if the array is sorted.
```js
Examples
search([1, 2, 3, 4], 3) ➞ 2

search([2, 4, 6, 8, 10], 8) ➞ 3

search([1, 3, 5, 7, 9], 11) ➞ -1
```
### :hocho:My Code
```js
const search = (arr, item) => arr.indexOf(item);
```

## Add, Subtract, Multiply or Divide?
Write a function that takes two numbers and returns if they should be added, subtracted, multplied or divided to get 24. If none of the operations can give 24, return null.
```
Examples
operation(15, 9) ➞ "added"

operation(26, 2) ➞ "subtracted"

operation(11, 11) ➞ null
```
### :syringe:My Code
```js
const operation= (num1, num2) =>
num1 + num2 == 24 ? "added" : num1*num2 == 24 ? "multiplied":
num1 - num2 == 24 ? "subtracted" : num1 / num2 == 24 ? "divided" : null;
```

