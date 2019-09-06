## Check if the String is a Palindrome
A palindrome is a word, phrase, number or other sequence of characters which reads the same backward or forward, such as madam or kayak.

Write a function that takes a string and determines whether it's a palindrome or not. The function should return a boolean (true or false value).
```js
Examples
isPalindrome("Neuquen") ➞ true

isPalindrome("Not a palindrome") ➞ false

isPalindrome("A man, a plan, a cat, a ham, a yak, a yam, a hat, a canal
```
### :evergreen_tree: My Code
```js
function isPalindrome(s) {
 s = s.toLowerCase().replace(/\W/gi,'');
  return s == [...s].reverse().join``;
}
```
