## Valid Zip Code
Zip codes consist of 5 consecutive digits. Given a string, write a function to determine whether the input is a valid zip code.
```js
Examples
isValid("59001") ➞ true

isValid("853a7") ➞ false

isValid("732 32") ➞ false

isValid("393939") ➞ false
```
### :scroll:My Code
```js
const isValid = zip => /\b\d{5}\b/g.test(zip);
```

## Bitwise Operations
A decimal number can be represented as a sequence of bits. To illustrate:
```
6  = 00000110
23 = 00010111
```
From the bitwise representation of numbers, we can calculate the bitwise AND, bitwise OR and bitwise XOR. Using the example above:
```js
bitwiseAND(6, 23)➞ 00000110
bitwiseOR(6, 23) ➞ 00010111
bitwiseXOR(6, 23) ➞ 00010001
```
Write 3 functions to calculate the bitwise AND, bitwise OR and bitwise XOR of two numbers.
```js
Examples
bitwiseAND(7, 12) ➞ 4

bitwiseOR(7, 12) ➞ 15

bitwiseXOR(7, 12) ➞ 11
```
### :clipboard:My Code
```js
const bitwiseAND = (n1, n2) => n1.toString() & n2.toString();
const bitwiseOR = (n1, n2) => n1 | n2;
const bitwiseXOR =(n1, n2) => n1 ^ n2;
```

## Recursion: Fibonacci Numbers
Fibonacci numbers are created in the following way:
```js
F(0) = 0
F(1) = 1
...
F(n) = F(n-2) + F(n-1)
```
Write a function that calculates the nth Fibonacci number.
```js
Examples
fib(0) ➞ 0

fib(1) ➞ 1

fib(2) ➞ 1

fib(8) ➞ 21
```
### :ledger:My Code
```js
const fib = n => n <= 1 ? n : fib(n-1) + fib(n-2);
```

## Recursion: Array Sum
Write a function that recursively finds the sum of an array.
```js
Examples
sum([1, 2, 3, 4]) ➞ 10

sum([1, 2]) ➞ 3

sum([1]) ➞ 1

sum([]) ➞ 0
```
### :books:My Code
```js
const sum = arr => arr.length === 0 ?  0 : arr[0] + sum(arr.slice(1));
```

## Factorial of a Positive Integer
Write a function that takes a positive integer and return its factorial.
```js
Examples
factorial(4) ➞ 24

factorial(0) ➞ 1

factorial(9) ➞ 362880
```
### :bookmark:My Code
```js
const factorial = z => z == 0 ? 1 : z * factorial(z-1);
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
### :name_badge:My Code
```js
const isSymmetrical = num =>
num == num.toString().split('').reverse().join('');
```
