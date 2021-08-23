## Is the String a Palindrome?

A palindrome is a word that is identical forward and backwards.
```
mom
racecar
kayak

Given a word, create a function that checks whether it is a palindrome.

Examples
checkPalindrome("mom") ➞ true

checkPalindrome("scary") ➞ false

checkPalindrome("reviver") ➞ true

checkPalindrome("stressed") ➞ false
```
### 🌇 My Code
```swift
let checkPalindrome:(String) -> Bool = {$0 == String($0.characters.reversed())}
```
