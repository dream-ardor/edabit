## Sort Numbers in Ascending Order

Create a function that takes an array of numbers and returns a new array, sorted in ascending order (smallest to biggest).
```
Rules
Sort numbers array in ascending order.
If functions argument is nil or an empty array, return an empty array.
Return new array of sorted numbers.

Examples
sortNumsAscending([1, 2, 10, 50, 5]) ➞ [1, 2, 5, 10, 50]

sortNumsAscending([80, 29, 4, -95, -24, 85]) ➞ [-95, -24, 4, 29, 80, 85]

sortNumsAscending(nil) ➞ []

sortNumsAscending([]) ➞ []
```
### 🌃 My Code
```swift
let sortNumsAscending:([Int]?) -> [Int] = {($0?.sorted())!}
```
