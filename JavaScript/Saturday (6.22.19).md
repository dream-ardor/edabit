## Get Student Names

Create a function that takes an array of students and returns an array of student names.
```js
Examples
getStudentNames([
  { name: "Steve" },
  { name: "Mike" },
  { name: "John" }
]) ➞ ["Steve", "Mike", "John"]
```
## My Code :computer:
```js
const getStudentNames = students => students.map(x => x.name);

```

## Filter by Digit Length
Create a function that filters out an array to include numbers who only have a certain number of digits.
```js
Examples
filterDigitLength([88, 232, 4, 9721, 555], 3) ➞ [232, 555]
// Include only numbers with 3 digits.

filterDigitLength([2, 7, 8, 9, 1012], 1) ➞ [2, 7, 8, 9]
// Include only numbers with 1 digit.

filterDigitLength([32, 88, 74, 91, 300, 4050], 1) ➞ []
// No numbers with only 1 digit exist => return empty array.

filterDigitLength([5, 6, 8, 9], 1) ➞ [5, 6, 8, 9]
// All numbers in the array have 1 digit only => return original array.
```
## My Code :raising_hand:
```js
function filterDigitLength(arr, num) {
 let foo = arr.map(String);
 return foo.filter(x=>x.length == num).map(Number); 
}
```

## Matchstick Houses
This challenge will help you interpret mathematical relationships both algebraically and geometrically.

Create a function that takes a number (step) as an argument and returns the amount of matchsticks in that step. See step 1, 2 and 3 in the image above.
```js
Examples
matchHouses(1) ➞ 6

matchHouses(4) ➞ 21

matchHouses(87) ➞ 436
```
## My Code :bulb:
```js
const matchHouses = step => step === 0 ? 0 : (step * 5) + 1;
```

## Check if a Number is a Palindrome
Write a function that returns true if a number is a palindrome.
```js
Examples
isPalindrome(838) ➞ true

isPalindrome(4433) ➞ false

isPalindrome(443344) ➞ true
```
## My Code :flashlight:	
```js
const isPalindrome = n =>
(n.toString() === n.toString().split("").reverse().join(""));
```

## Hamming Distance
Hamming distance is the number of characters that differ between two strings.

To illustrate:

String1: "abcbba"
String2: "abcbda"

Hamming Distance: 1 - "b" vs. "d" is the only difference.
Create a function that computes the hamming distance between two strings.
```js
Examples
hammingDistance("abcde", "bcdef") ➞ 5

hammingDistance("abcde", "abcde") ➞ 0

hammingDistance("strong", "strung") ➞ 1
```

## My Code :spades:
```js
function hammingDistance(str1, str2) {
  let distance = 0;
  for (let i = 0; i < str1.length; i += 1) {
    if (str1[i] !== str2[i]) {
      distance += 1;
    }
  }
  return distance;
}
```


