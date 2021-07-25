## How Much is True?

Create a function which returns the number of true values there are in an array.
```swift
Examples
countTrue([true, false, false, true, false]) ➞ 2

countTrue([false, false, false, false]) ➞ 0

countTrue([]) ➞ 0
```
### 🏜️ My Code
```swift
func countTrue(_ a: [Bool]) -> Int {
  return a.filter{$0}.count;
}

or

let countTrue = {(a: [Bool]) in a.filter{$0 == true}.count}
```
