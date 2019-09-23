## Seconds in Hours
Write a function that converts hours into seconds.
```js
Examples
howManySeconds(2) ➞ 7200

howManySeconds(10) ➞ 36000

howManySeconds(24) ➞ 86400
```
### :leaves: My Code
```js
const howManySeconds = h => h * 3600;
```

## Convert a Number to Base 2
Create a function that returns a base 2 (binary) represetation of a base 10 (decimal) number. To convert is simple: ((2) means base 2 and (10) means base 10) 010101001(2) = 1 + 8 + 32 + 128.

Going from right to left, the value of the most right bit is 1, now from that every bit to the left will be x2 the value, value of an 8 bit binary numbers are (256, 128, 64, 32, 16, 8, 4, 2, 1).
```js
Examples
binary(1) ➞ 1
// 1*1 = 1

binary(5) ➞ 101
// 1*1 + 1*4 = 5

binary(10) ➞ 1010
// 1*2 + 8*2 = 5
```
### :leaves: My Code
```js
const binary = d => d.toString(2);
```

## Reverse the Number
Create a function that takes an integer n and reverses it.
```
Examples
rev(5121) ➞ "1215"

rev(69) ➞ "96"

rev(-122157) ➞ "751221"
```
### :leaves: My Code
```js
const rev = n => 
 Math.abs(n).toString().split('').reverse().join('');
```

## Basic Calculator
Create a function that takes two numbers and a mathematical operator + - / * and will perform a calculation with the given numbers.
```js
Examples
calculator(2, "+", 2) ➞ 4

calculator(2, "*", 2) ➞ 4

calculator(4, "/", 2) ➞ 2
```
### :leaves: My Code
```js
const calculator = (n1, o, n2) =>
n2 == 0 ? "Can't divide by 0!" :
o == '/' ? n1 /n2 :
o == '-' ? n1 - n2:
o == '*' ? n1 * n2:
n1 + n2;
```

