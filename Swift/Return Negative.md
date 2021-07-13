## Return Negative

Create a function that takes a number as an argument and returns negative of that number. Return negative numbers without any change.
```swift
Examples
returnNegative(4) ➞ -4

returnNegative(15) ➞ -15

returnNegative(-4) ➞ -4

returnNegative(0) ➞ 0
```
### 💻 My Code
```swift
let returnNegative = {$0 > 0 ? $0 * -1 : $0}
```
