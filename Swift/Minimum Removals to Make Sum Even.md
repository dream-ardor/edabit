## Minimum Removals to Make Sum Even

Create a function that returns the minimum number of removals to make the sum of all elements in an array even.
```swift
Examples
minimumRemovals([1, 2, 3, 4, 5]) ➞ 1

minimumRemovals([5, 7, 9, 11]) ➞ 0

minimumRemovals([5, 7, 9, 12]) ➞ 1
```
### 🎚️ My Code
```swift
let minimumRemovals:([Int]) -> Int = {$0.reduce(0,+) % 2}
```
