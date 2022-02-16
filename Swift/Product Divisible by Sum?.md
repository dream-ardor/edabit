## Product Divisible by Sum?

Write a function that returns true if the product of an array is divisible by the sum of that same array. Otherwise, return false.
```swift
Examples
divisible([3, 2, 4, 2]) ➞ false

divisible([4, 2, 6]) ➞ true
// 4 * 2 * 6 / (4 + 2 + 6)

divisible([3, 5, 1]) ➞ false
```
### 🦯 My Code
```swift
let divisible = {(a:[Int]) in  a.reduce(1,*) % a.reduce(0,+) == 0}
```
