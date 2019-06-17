## Palindrome?

A palindrome is a word that is identical forward and backwards.
```js
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

## My Code
```js
//short code
const checkPalindrome = str => str == str.split('').reverse().join('') ? true : false;

//for loop
function fastestIsPalindrome(str) {
  var len = Math.floor(str.length / 2);
  for (var i = 0; i < len; i++)
    if (str[i] !== str[str.length - i - 1])
      return false;
  return true;
}

//alternative approach
function checkPalindrome(str) {
  /* remove special characters, spaces and make lowercase */
  let removeChar = str.replace(/[^A-Z0-9]/ig, "").toLowerCase();

  /* reverse removeChar variable for comparison */
  let checkPalindrome = removeChar.split('').reverse().join('');

  /* Check to see if str is a Palindrome */
   return (removeChar === checkPalindrome);
}

```
