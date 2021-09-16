## Absolute Sum

Take an array of integers (positive or negative or both) and return the sum of the absolute value of each element.
```swift
Examples
getAbsSum([2, -1, 4, 8, 10]) ➞ 25

getAbsSum([-3, -4, -10, -2, -3]) ➞ 22

getAbsSum([2, 4, 6, 8, 10]) ➞ 30

getAbsSum([-1]) ➞ 1
```
### 🎋 My Code
```swift
let getAbsSum:([Int]) -> Int = {$0.map{abs($0)}.reduce(0,+)}
```
