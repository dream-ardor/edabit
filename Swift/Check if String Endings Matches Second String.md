## Check if String Ending Matches Second String

Create a function that takes two strings and returns true if the first string ends with the second string; otherwise return false.
```swift
Examples
checkEnding("abc", "bc") ➞ true

checkEnding("abc", "d") ➞ false

checkEnding("samurai", "zi") ➞ false

checkEnding("feminine", "nine") ➞ true

checkEnding("convention", "tio") ➞ false
```
### 🔚 My Code
```swift
let checkEnding:(String,String) -> Bool = {$0.hasSuffix($1)}
```
