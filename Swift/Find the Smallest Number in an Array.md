## Find the Smallest Number in an Array

Create a function that takes an array of numbers and returns the smallest number in the set.
```swift
Examples
findSmallestNum([34, 15, 88, 2]) ➞ 2

findSmallestNum([34, -345, -1, 100]) ➞ -345

findSmallestNum([-76, 1.345, 1, 0]) ➞ -76

findSmallestNum([0.4356, 0.8795, 0.5435, -0.9999]) ➞ -0.9999

findSmallestNum([7, 7, 7]) ➞ 7
```
### 🌴 My Code
```swift
let findSmallestNum = {(a:[Double]) in a.min()!}
```
