## Product of All Odd Integers

Create a function that returns the product of all odd integers in an array.
```swift
Examples
oddProduct([3, 4, 1, 1, 5]) ➞ 15

oddProduct([5, 5, 8, 2, 4, 32]) ➞ 25

oddProduct([1, 2, 1, 2, 1, 2, 1, 2]) ➞ 1
```
### 🌆 My Code
```swift
let oddProduct:([Int]) -> Int = {$0.filter{!($0 % 2 == 0)}.reduce(1, *)}
```
