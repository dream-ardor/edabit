## Missing Letters

Given a string containing unique letters, return a sorted string with the letters that don't appear in the string.
```js
Examples
getMissingLetters("abcdefgpqrstuvwxyz") ➞ "hijklmno"

getMissingLetters("zyxwvutsrq") ➞ "abcdefghijklmnop"

getMissingLetters("abc") ➞ "defghijklmnopqrstuvwxyz"

getMissingLetters("abcdefghijklmnopqrstuvwxyz") ➞ ""
```
### :computer: My Code
```js
const getMissingLetters = s => [...'abcdefghijklmnopqrstuvwxyz'].filter(e => !s.includes(e)).join('');


//alternate solution
const getMissingLetters = s => {
  let a = "abcdefghijklmnopqrstuvwxyz";
   s = s.replace(/[^a-z]/ig, "").toLowerCase();
   s = a.split('').filter(b => (s.indexOf(b) == -1));
  return s.join('')};
```
