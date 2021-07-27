## Eliminate Odd Numbers within an Array

Create a function that takes an array of numbers and returns only the even values.
```swift
Examples
noOdds([1, 2, 3, 4, 5, 6, 7, 8]) ➞ [2, 4, 6, 8]

noOdds([43, 65, 23, 89, 53, 9, 6]) ➞ [6]

noOdds([718, 991, 449, 644, 380, 440]) ➞ [718, 644, 380, 440]
```
###  🌧️ My Code
```swift
func noOdds(_ a: [Int]) -> [Int] {
  return a.filter{$0 % 2 == 0};
}
```
