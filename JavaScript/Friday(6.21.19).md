## Convert Number to Corresponding Month Name

Create a function that takes a number (from 1 to 12) and return its corresponding month name as a string.
```js
Examples
month_name(3) ➞ "March"

month_name(12) ➞ "December"

month_name(6) ➞ "June"
```
## My Code :unlock:
```js
const month_name = x => 
['January', 'February', 'March', 'April',
'May', 'June', 'July', 'August', 'September', 
'October', 'November', 'December'][x - 1];
```

## Between Words 
Write a function that returns true if a word can be found in between the start and end word in a dictionary.
```js
isBetween(start_word, end_word, word)

Examples
isBetween("apple", "banana", "azure") ➞ true

isBetween("monk", "monument", "monkey") ➞ true

isBetween("bookend", "boolean", "boost") ➞ false
```
## My Code :lock_with_ink_pen:
```js
const isBetween = (first, last, word) =>  word > first & word < last ? true : false;

```

## Next Element in Arithmetic Sequence 
Create a function that returns the next element in an arithmetic sequence. In an arithmetic sequence, each element is formed by adding the same constant to the previous element.
```js
Examples
nextElement([3, 5, 7, 9]) ➞ 11

nextElement([-5, -6, -7]) ➞ -8

nextElement([2, 2, 2, 2, 2]) ➞ 2
```
## My Code :lock:
```js
const nextElement = arr => arr.pop() + arr[1] - arr[0];
```

## Palindrome?
A palindrome is a word that is identical forward and backwards.
```
mom
racecar
kayak
```
Given a word, create a function that checks whether it is a palindrome.
```js
Examples
checkPalindrome("mom") ➞ true

checkPalindrome("scary") ➞ false

checkPalindrome("reviver") ➞ true

checkPalindrome("stressed") ➞ false
```
## My Code :closed_lock_with_key:
```js
function checkPalindrome(str) {
	let regex = str.replace(/[^A-Z0-9]/ig, "").toLowerCase();
	let check = regex.split("").reverse().join("");
	return (regex === check);
}
```

## Even Number Generator
Create a function that finds all even numbers from 1 to the given number.
```js
Examples:
findEvenNums(8) ➞ [2, 4, 6, 8]

findEvenNums(4) ➞ [2, 4]

findEvenNums(2) ➞ [2]
```
## My Code :key:
```js
function findEvenNums(num) {
 let n1 = [];
 for(i = 2; i <=num; i+=2) {
   n1.push(i)
 }
return n1;
}
```

