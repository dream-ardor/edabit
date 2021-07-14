## Two Makes Ten

Create a function that takes two arguments. Both arguments are integers, a and b. Return true if one of them is 10 or if their sum is 10.
```swift
Examples
makesTen(9, 10) ➞ true

makesTen(9, 9) ➞ false

makesTen(1, 9) ➞ true
```
### 🌴 My Code
```swift
let makesTen = {$0 == 10 || $1 == 10 || $0 + $1 == 10}
```
