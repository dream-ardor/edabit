## Nth Smallest Integer

Given an unsorted array, create a function that returns the nth smallest integer (the smallest integer is the first smallest, the second smallest integer is the second smallest, etc).
```swift
Examples
nthSmallest([1, 3, 5, 7], 1) ➞ 1

nthSmallest([1, 3, 5, 7], 3) ➞ 5

nthSmallest([1, 3, 5, 7], 5) ➞ nil

nthSmallest([7, 3, 5, 1], 2) ➞ 3
```
### 🔄 My Code
```swift
let nthSmallest:([Int],Int) -> Int?  = {$0.count < $1 ? nil :  $0.sorted()[$1-1]}
```
