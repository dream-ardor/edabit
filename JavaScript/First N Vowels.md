## First N Vowels

Write a function that returns the first n vowels of a string.
```js
Examples
firstNVowels("sharpening skills", 3) ➞ "aei"

firstNVowels("major league", 5) ➞ "aoeau"

firstNVowels("hostess", 5) ➞ "invalid"

Notes:
Return "invalid" if the n exceeds the number of vowels in a string.
Vowels are: a, e, i, o, u
```
### :computer: My Code
```js
const firstNVowels = (s, n) => {
 let a = s.match(/[aeiou]/g).join('').slice(0,n);
  return a.length == n ? a:'invalid';
}
```
