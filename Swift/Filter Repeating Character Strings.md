## Filter Repeating Character Strings

Create a function that keeps only strings with repeating identical characters (in other words, it has a set size of 1).
```swift
Examples
identicalFilter(["aaaaaa", "bc", "d", "eeee", "xyz"])
➞ ["aaaaaa", "d", "eeee"]

identicalFilter(["88", "999", "22", "545", "133"])
➞ ["88", "999", "22"]

identicalFilter(["xxxxo", "oxo", "xox", "ooxxoo", "oxo"])
➞ []
```
### 🗃️ My Code
```swift
let identicalFilter:([String]) -> [String] = {$0.filter{Set($0.characters).count == 1}}
```
