## Total Number of Unique Characters

Given two strings, create a function that returns the total number of unique characters from the combined string.
```
Examples
countUnique("apple", "play") ➞ 5
// "appleplay" has 5 unique characters:
// "a", "e", "l", "p", "y"

countUnique("sore", "zebra") ➞ 7
// "sorezebra" has 7 unique characters:
// "a", "b", "e", "o", "r", "s", "z"

countUnique("a", "soup") ➞ 5
```
### 🌵 My Code
```swift
let countUnique:(String,String) -> Int = {Set(($0+$1).characters).count}
```
