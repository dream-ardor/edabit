## Word Endings

Create a function that adds a string ending to each member in an array.
```swift
Examples
addEnding(["clever", "meek", "hurried", "nice"], "ly")
➞ ["cleverly", "meekly", "hurriedly", "nicely"]

addEnding(["new", "pander", "scoop"], "er")
➞ ["newer", "panderer", "scooper"]

addEnding(["bend", "sharpen", "mean"], "ing")
➞ ["bending", "sharpening", "meaning"]
```
### 🏛️ My Code
```swift
let addEnding = {(a:[String], b:String) in a.map{$0 + b}}
```
