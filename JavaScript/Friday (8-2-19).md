## ATM PIN Code Validation
ATM machines allow 4 or 6 digit PIN codes and PIN codes cannot contain anything but exactly 4 digits or exactly 6 digits. Your task is to create a function that takes a string and returns true if the PIN is valid and false if it's not.
```js
Examples
validatePIN("1234") ➞ true

validatePIN("12345") ➞ false

validatePIN("a234") ➞ false

validatePIN("") ➞ false
```
### :u6307:My Code
```js
const validatePIN = pin => /^(\d{4}|\d{6})$/.test(pin);
```
## No Conditionals?
Write a function that returns 0 if the input is 1, and returns 1 if the input is 0.
```js
Examples
flip(1) ➞ 0

flip(0) ➞ 1
```
```
Notes
Bonus: Do this without using any:

- conditionals or ternary operators.
- negations.
- bit operators.
```
### :u6307:My Code
```js
const flip = y => [1,0][y];
```

## Negative Image
Suppose an image can be represented as a 2D array of 0s and 1s.

Write a function to reverse an image. Replace the 0s with 1s and vice versa.
```js
Examples
reverseImage([
  [1, 0, 0],
  [0, 1, 0],
  [0, 0, 1]
]) ➞ [
  [0, 1, 1],
  [1, 0, 1],
  [1, 1, 0]
]

reverseImage([
  [1, 1, 1],
  [0, 0, 0]
]) ➞ [
  [0, 0, 0],
  [1, 1, 1]
]

reverseImage([
  [1, 0, 0],
  [1, 0, 0]
]) ➞ [
  [0, 1, 1],
  [0, 1, 1]
]
```
### :u6307:My Code
```js
const reverseImage = image => image.map(x => x.map(y => y == 1 ? 0 : 1));
```
## Basic E-Mail Validation
Create a function that accepts a string, checks if it's a valid email address and returns either true or false, depending on the evaluation.
```
The string must contain an @ character.
The string must contain a . character.
The @ must have at least one character in front of it.
e.g. "e@edabit.com" is valid while "@edabit.com" is invalid.
The . and the @ must be in the appropriate places.
e.g. "hello.email@com" is invalid while "john.smith@email.com" is valid.
If the string passes these tests, it's considered a valid email address.
```
```js
Examples
validateEmail("@gmail.com") ➞ false

validateEmail("hello.gmail@com") ➞ false

validateEmail("gmail") ➞ false

validateEmail("hello@gmail") ➞ false

validateEmail("hello@edabit.com") ➞ true
```
### :u6307:My Code
```js
const validateEmail = str => str.indexOf("@") > 0 && str.endsWith(".com");

//regex
const validateEmail = str => /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(str);
```



