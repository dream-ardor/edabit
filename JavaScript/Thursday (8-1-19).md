## Basic Statistics: Mean
The mean of a group of numbers is calculated by summing all numbers, and dividing this sum by the total count of numbers in the group. Given a sorted array of numbers, return the mean (rounded to one decimal place).
```js
Examples
mean([1, 6, 6, 7, 8, 8, 9, 10, 10]) ➞ 7.2 

mean([1, 3, 8, 9, 9, 10]) ➞ 6.7

mean([2, 3, 3, 6, 6, 8, 9, 10]) ➞ 5.9 
```
### :ledger:My Code
```js
const mean = nums => +(nums.reduce((a,b)=> a+b) / nums.length).toFixed(1);
```

## Re-Form The Word
A word has been split into a left part and a right part. Re-form the word by adding both halves together, changing the first character to an uppercase letter.
```js
Examples
getWord("seas", "onal") ➞ "Seasonal"

getWord("comp", "lete") ➞ "Complete"

getWord("lang", "uage") ➞ "Language"
```
### :ledger:My Code
```js
const getWord = (left, right) => left.charAt(0).toUpperCase() + left.substr(1) + right;
```

## The Perrin Sequence
Each number in the Perrin sequence is created by summing the numbers two positions and three positions before it. The first three numbers are (3, 0, 2), and the sequence is extended as follows:

P(0) P(1) P(2) P(3) P(4) P(5) P(6) P(7) ... P(n)
  3,   0,   2,   3,   2,   5,   5,   7, ...
Given a value for n, return the Perrin number P(n).
```js
Examples
perrin(1) ➞ 0

perrin(8) ➞ 10

perrin(26) ➞ 1497
```
### :ledger:My Code
```js
function perrin(n) {
	let a = 3; let b = 0; let c = 2;
 if (n == 0) 
        return a; 
    if (n == 1) 
        return b; 
    if (n == 2) 
        return c; 
    while (n > 2) { 
        m = a + b; 
        a = b; 
        b = c; 
        c = m; 
        n--; 
    } 
    return m; 
}

//recursively
function perrin(n) {
  if (n == 0) return 3; 
  if (n == 1) return 0; 
  if (n == 2) return 2; 
  return perrin(n - 2) + perrin(n - 3);    
}

```

## Unlucky 13
Given a sorted array of numbers, remove any numbers that are divisible by 13. Return the amended array.
```js
Examples
unlucky13([53, 182, 435, 591, 637]) ➞ [53, 435, 591]
# 182 and 637 are divisible by 13

unlucky13([24, 316, 393, 458, 1279]) ➞ [24, 316, 393, 458, 1279]
# no numbers in the array are divisible by 13

unlucky13([104, 351, 455, 806, 871]) ➞ []
# all numbers in the array are divisible by 13
```
### :ledger:My Code
```js
const unlucky13 = nums => nums.filter(x => x % 13 !== 0);
```
## ATM PIN Code Validation
ATM machines allow 4 or 6 digit PIN codes and PIN codes cannot contain anything but exactly 4 digits or exactly 6 digits. Your task is to create a function that takes a string and returns true if the PIN is valid and false if it's not.
```js
Examples
validatePIN("1234") ➞ true

validatePIN("12345") ➞ false

validatePIN("a234") ➞ false

validatePIN("") ➞ false
```
### :ledger:My Code
```js
const validatePIN = pin => /^(\d{4}|\d{6})$/.test(pin);
```




