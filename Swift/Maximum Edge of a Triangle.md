## Maximum Edge of a Triangle

Create a function that finds the maximum range of a triangle's third edge, where the side lengths are all integers.
```swift
Examples
nextEdge(8, 10) ➞ 17

nextEdge(5, 7) ➞ 11

nextEdge(9, 2) ➞ 10
```
### 📐 My Code
```swift
let nextEdge = {(a: Int,b: Int) in a + b - 1}

//alternate solution
let nextEdge: (Int, Int) -> Int = { $0 + $1 - 1 }
```
