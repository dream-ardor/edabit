## Reverse the Number
Create a function that takes an integer n and reverses it.
```js
Examples
rev(5121) ➞ "1215"

rev(69) ➞ "96"

rev(-122157) ➞ "751221"
```
### :file_cabinet:	My Code
```js
const rev = n => [...''+Math.abs(n)].reverse``.join``;

//alternate way
const rev = n => String(Math.abs(n)).split('').reverse().join('');
```

## Basic Calculator
Create a function that takes two numbers and a mathematical operator + - / * and will perform a calculation with the given numbers.
```js
Examples
calculator(2, "+", 2) ➞ 4

calculator(2, "*", 2) ➞ 4

calculator(4, "/", 2) ➞ 2
```
Notes
If the input tries to divide by 0, return: "Can't divide by 0!"
### :file_cabinet: My Code
```js
const calculator = (n1, o, n2) => n2 == 0 ? "Can't divide by 0!" :
o == '/' ? n1 / n2 :
o == '-' ? n1 - n2 :
o == '*' ? n1 * n2 : n1 + n2;
```

## Change Every Letter to the Next Letter
Write a function that changes every letter to the next letter:
```js
"a" becomes "b"
"b" becomes "c"
"d" becomes "e"
and so on ...
```
```js
Examples
move("hello") ➞ "ifmmp"

move("bye") ➞ "czf"

move("welcome") ➞ "xfmdpnf"
```
### :file_cabinet: My Code
```js
const move = w =>  
[...w].map(a => String.fromCharCode(a.charCodeAt(0) + 1)).join``;
```

## Seven Boom!
Create a function that takes an array of numbers and return "Boom!" if the number 7 appears in the array. Otherwise, return "there is no 7 in the array".
```
Examples
sevenBoom([1, 2, 3, 4, 5, 6, 7]) ➞ "Boom!"

sevenBoom([8, 6, 33, 100]) ➞ "there is no 7 in the array"

sevenBoom([2, 55, 60, 97, 86]) ➞ "Boom!"
```
### :file_cabinet: My Code
```js
const sevenBoom = a =>
 a.toString().includes(7) ? "Boom!" : "there is no 7 in the array";
```
## Compounding Letters
Create a function that takes a string and returns a new string with each new character accumulating by +1. Separate each set with a dash.
```js
Examples
accum("abcd") ➞ "A-Bb-Ccc-Dddd"

accum("RqaEzty") ➞ "R-Qq-Aaa-Eeee-Zzzzz-Tttttt-Yyyyyyy"
```
### :file_cabinet:My Code
```js
const accum = s => [...s].map((a,b)=>
a.toUpperCase() + a.toLowerCase().repeat(b)).join`-`;
```


