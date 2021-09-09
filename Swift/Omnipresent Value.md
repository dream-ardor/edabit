## Omnipresent Value

A value is omnipresent if it exists in every subarray inside the main array.

To illustrate:
```
[[3, 4], [8, 3, 2], [3], [9, 3], [5, 3], [4, 3]]
// 3 exists in every element inside this array, so is omnipresent.
Create a function that determines whether an input value is omnipresent for a given array.
```
```swift
Examples
isOmnipresent([[1, 1], [1, 3], [5, 1], [6, 1]], 1) ➞ true

isOmnipresent([[1, 1], [1, 3], [5, 1], [6, 1]], 6) ➞ false

isOmnipresent([[5], [5], [5], [6, 5]], 5) ➞ true

isOmnipresent([[5], [5], [5], [6, 5]], 6) ➞ false
```
### 🌇 My Code
```swift
func isOmnipresent(_ a: [[Int]], _ v: Int) -> Bool {
  return a.filter{$0.contains(v)}.count > 1
}
```
