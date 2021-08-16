## Even Number Generator

Create a function that finds all even numbers from 1 to the given number.
```swift
Examples
findEvenNums(8) ➞ [2, 4, 6, 8]

findEvenNums(4) ➞ [2, 4]

findEvenNums(2) ➞ [2]
```
### 🎚️ My Code
```swift
let findEvenNums = {(n: Int) in (1...n).filter {$0 % 2 == 0}}
```
