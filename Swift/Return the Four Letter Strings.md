## Return the Four Letter Strings

Create a function that takes an array of strings and returns the words that are exactly four letters.
```swift
Examples
isFourLetters(["Tomato", "Potato", "Pair"]) ➞ ["Pair"]

isFourLetters(["Kangaroo", "Bear", "Fox"]) ➞ ["Bear"]

isFourLetters(["Ryan", "Kieran", "Jason", "Matt"]) ➞ ["Ryan", "Matt"]
```
## 🏜️ My Code
```swift
let isFourLetters = {(a:[String]) in a.filter{ $0.characters.count == 4} }
```




