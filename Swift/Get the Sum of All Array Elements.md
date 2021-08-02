## Get the Sum of All Array Elements

Create a function that takes an array and returns the sum of all numbers in the array.
```swift
Examples
getSum(of: [2, 7, 4]) ➞ 13

getSum(of: [45, 3, 0]) ➞ 48

getSum(of: [-2, 84, 23]) ➞ 105
```
### ➕ My Code
```swift
func getSum(of i: [Int]) -> Int {
  return i.reduce(0, +);	
}
```
