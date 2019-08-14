## Is the Word an Isogram?
An isogram is a word that has no repeating letters, consecutive or nonconsecutive. Create a function that takes a string and returns either true or false depending on whether or not it's an "isogram".
```js
Examples
isIsogram("Algorism") ➞ true

isIsogram("PasSword") ➞ false (not case sensitive)

isIsogram("Consecutive") ➞ false
```

### :stars:My Code
```js
const isIsogram = str => !/(\w).*\1/i.test(str);
```

## Stretched Words
Write a function that takes a string, and returns a new string with any duplicate consecutive letters removed.
```js
Examples
unstretch("ppoeemm") ➞ "poem"

unstretch("wiiiinnnnd") ➞ "wind"

unstretch("ttiiitllleeee") ➞ "title"

unstretch("cccccaaarrrbbonnnnn") ➞ "carbon"
```
### :stars:My Code
```js
const unstretch = word => word.replace(/(.)\1+/g, '$1');
```

## Find the Characters Counterpart Char Code
Create a function that takes a single character as an argument and returns the char code of its lowercased / uppercased counterpart.
```js
Examples
Given that:
  - "A" char code is: 65
  - "a" char code is: 97

counterpartCharCode("A") ➞ 97

counterpartCharCode("a") ➞ 65
```
### :stars:My Code
```js
const counterpartCharCode = c => c === c.toUpperCase() ? c.toLowerCase().charCodeAt():
c.toUpperCase().charCodeAt();
```
## The 3 Programmers Problem
You hired three programmers and you (hopefully) pay them. Create a function that takes three numbers (the hourly wage of each programmer) and returns the difference between the highest-paid programmer and the lowest-paid.
```js
Examples
programmers(147, 33, 526) ➞ 493

programmers(33, 72, 74) ➞ 41

programmers(1, 5, 9) ➞ 8
```
### :stars:My Code
```js
const programmers = (o,t,th) => Math.max(o,t,th) - Math.min(o,t,th);
```
## Recursion: Fibonacci Numbers
Fibonacci numbers are created in the following way:
```
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
### :stars:My Code
```js
const fib = n => n <= 1 ? n : fib(n-1) + fib(n-2);
```




