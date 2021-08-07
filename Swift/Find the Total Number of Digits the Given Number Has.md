## Find the Total Number of Digits the Given Number Has

Create a function that takes a number as an argument and returns the amount of digits it has.
```swift
Examples
findDigitAmount(123) ➞ 3

findDigitAmount(56) ➞ 2

findDigitAmount(7154) ➞ 4

findDigitAmount(61217311514) ➞ 11

findDigitAmount(0) ➞ 1
```
### 🗂️ My Code
```swift
let findDigitAmount:(Int) -> Int = {String($0).characters.count}
```
