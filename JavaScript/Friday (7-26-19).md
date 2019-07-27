## Limit a Number's Value
Create a function that takes three number arguments - one number as an input, and two additional numbers representing the endpoints of a closed range - and return the number limited to this range.

If the number falls within the range, the number should be returned.
If the number is less than the lower limit of the range, the lower limit should be returned.
If the number is greater than the upper limit of the range, the upper limit should be returned.
```js
Examples
limitNumber(5, 1, 10) ➞ 5

limitNumber(-3, 1, 10) ➞ 1

limitNumber(14, 1, 10) ➞ 10

limitNumber(4.6, 1, 10) ➞ 4.6
```
### My Code
```js
let limitNumber = (num, low, high) => num < low ? low : num > high ? high : num;
```

## Double Letters
Create a function that takes a word and returns true if the word has two consecutive identical letters.
```js
Examples
doubleLetters("loop") ➞ true

doubleLetters("yummy") ➞ true

doubleLetters("orange") ➞ false

doubleLetters("munchkin") ➞ false
```
### My Code
```js
const doubleLetters = w =>/(.)\1/g .test(w);

//another slightly different regex solution
let doubleLetters = word => /(\w)\1+/.test(word);
```

## Purge and Organize
Given an array of numbers, write a function that returns an array that...

Has all duplicate elements removed.
Is sorted from least to greatest value.
```js
Examples
uniqueSort([1, 2, 4, 3]) ➞ [1, 2, 3, 4]

uniqueSort([1, 4, 4, 4, 4, 4, 3, 2, 1, 2]) ➞ [1, 2, 3, 4]

uniqueSort([6, 7, 3, 2, 1]) ➞ [1, 2, 3, 6, 7]
```
### My Code
```js
const uniqueSort = arr => [...new Set(arr)].sort((a,b)=> a-b);
```

## Recursion: String Palindromes
Write a function that recursively determines if a string is a palindrome.
```js
Examples
isPalindrome("abcba") ➞ true

isPalindrome("b") ➞ true

isPalindrome("") ➞ true

isPalindrome("ad") ➞ false
```

### My Code
```js
const isPalindrome = str => str.length < 2 ? true : str.endsWith(str[0]) ? isPalindrome(str.slice(1,-1)) : false;
```

