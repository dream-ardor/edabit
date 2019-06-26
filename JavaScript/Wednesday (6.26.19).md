## Flip the Boolean
Create a function that reverses a boolean value and returns the string "boolean expected" if another variable type is given.
```js
Examples
reverse(true) ➞ false

reverse(false) ➞ true

reverse(0) ➞ "boolean expected"

reverse(null) ➞ "boolean expected"
```
### My Code :trophy:
```js
const reverse = bool => 
bool === true ? false : bool === false ? true : 'boolean expected';
```

## Check if a Number is a Palindrome
Write a function that returns true if a number is a palindrome.
```js
Examples
isPalindrome(838) ➞ true

isPalindrome(4433) ➞ false

isPalindrome(443344) ➞ true
```
### My Code :gem:
```js
const isPalindrome = n => n == n.toString().split('').reverse().join('') ? true : false;
```

## Lexicographically First and Last

Write a function that returns the lexicographically first and lexicographically last rearrangements of a string. Output the results in the following manner:
```js
firstAndLast(string) ➞ [first, last]
Examples
firstAndLast("marmite") ➞ ["aeimmrt", "trmmiea"]

firstAndLast("bench") ➞ ["bcehn", "nhecb"]

firstAndLast("scoop") ➞ ["coops", "spooc"]
```
### My Code :clubs:
```js
const firstAndLast = s => [s.split('').sort().join(''),
s.split('').sort().reverse().join('')];
```
## Multiply by Length
Create a function to multiply all values in an array by the amount of values in that array.
```js
Examples
MultiplyByLength([2, 3, 1, 0]) ➞ [8, 12, 4, 0]

MultiplyByLength([4, 1, 1]) ➞ ([12, 3, 3])

MultiplyByLength([1, 0, 3, 3, 7, 2, 1]) ➞  [7, 0, 21, 21, 49, 14, 7]

MultiplyByLength([0]) ➞ ([0])
```
### My Code :diamonds:
```js
const MultiplyByLength = arr => arr.map(x => x * arr.length);
```
