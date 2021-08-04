## Find the Index

Create a function that takes an array and a string as arguments and return the index of the string.
```swift
Examples
find_index(["hi", "edabit", "fgh", "abc"], "fgh") ➞ 2

find_index(["Red", "blue", "Blue", "Green"], "blue") ➞ 1

find_index(["a", "g", "y", "d"], "d") ➞ 3

find_index(["Pineapple", "Orange", "Grape", "Apple"], "Pineapple") ➞ 0
```
### 🕋 My Code
```swift
let find_index:([String],String) -> Int = {$0.index(of:$1)!} 
```
