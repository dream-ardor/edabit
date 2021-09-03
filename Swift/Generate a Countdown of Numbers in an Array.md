## Generate a Countdown of Numbers in an Array

Create a function that takes a number as an argument and returns an array of numbers counting down from this number to zero.
```swift
Examples
countdown(5) ➞ [5, 4, 3, 2, 1, 0]

countdown(1) ➞ [1, 0]

countdown(0) ➞ [0]
```
### 🉑 My Code
```swift
let countdown:(Int) -> [Int] = {Array(0...$0).reversed()}
```
