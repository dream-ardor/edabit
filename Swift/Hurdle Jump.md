## Hurdle Jump

Create a function that takes an array of hurdle heights and a jumper's jump height, and determine whether or not the hurdler can clear all the hurdles.

A hurdler can clear a hurdle if their jump height is greater than or equal to the hurdle height.
```swift
Examples
hurdleJump([1, 2, 3, 4, 5], 5) ➞ true

hurdleJump([5, 5, 3, 4, 5], 3) ➞ false

hurdleJump([5, 4, 5, 6], 10) ➞ true

hurdleJump([1, 2, 1], 1) ➞ false

Notes
Return true for the edge case of an empty array of hurdles. (Zero hurdles means that any jump height can clear them).
```
### :computer: My Code
```swift
func hurdleJump(_ h: [Int], _ j: Int) -> Bool {
 return h.max() ?? 0 <= j;
}

//alternate solutions

let hurdleJump =  {(a:[Int],b:Int) in a.max() ?? 0 <= b}

let hurdleJump =  {(a:[Int],b:Int) in a.filter{$0 < b}.count > 0 || a == []}
```
