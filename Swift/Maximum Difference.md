## Maximum Difference

Given a list of integers, return the difference between the largest and smallest integers in the list.
```swift
Examples
difference([10, 15, 20, 2, 10, 6]) ➞ 18
// 20 - 2 = 18

difference([-3, 4, -9, -1, -2, 15]) ➞ 24
// 15 - (-9) = 24

difference([4, 17, 12, 2, 10, 2]) ➞ 15
```
### 🐱 My Code
```swift
let difference:([Int]) -> Int = {$0.max()! - $0.min()!}
```
