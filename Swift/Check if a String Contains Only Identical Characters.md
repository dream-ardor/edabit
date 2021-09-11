## Check if a String Contains only Identical Characters

Write a function that returns true if all characters in a string are identical and false otherwise.
```swift
Examples
isIdentical("aaaaaa") ➞ true

isIdentical("aabaaa") ➞ false

isIdentical("ccccca") ➞ false

isIdentical("kk") ➞ true
```
### 🪐 My Code
```swift
let isIdentical:(String) -> Bool = {Set($0.characters).count == 1}
```
