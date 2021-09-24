## Factorize a Number

Create a function that takes a number as its argument and returns an array of all its factors.
```swift
Examples
factorize(12) ➞ [1, 2, 3, 4, 6, 12]

factorize(4) ➞ [1, 2, 4]

factorize(17) ➞ [1, 17]
```
### 🏹 My Code
```swift
func factorize(_ n: Int) -> [Int] {
  return Array(1...n).filter{n % $0 == 0}
}
```
