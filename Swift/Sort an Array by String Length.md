## Sort an Array by String Length

Create a function that takes an array of strings and return an array, sorted from shortest to longest.
```swift
Examples
sortByLength(["Google", "Apple", "Microsoft"])
➞ ["Apple", "Google", "Microsoft"]

sortByLength(["Leonardo", "Michelangelo", "Raphael", "Donatello"])
➞ ["Raphael", "Leonardo", "Donatello", "Michelangelo"]

sortByLength(["Turing", "Einstein", "Jung"])
➞ ["Jung", "Turing", "Einstein"]
```
### ⚜️ My Code
```swift
let sortByLength:([String]) -> [String] = {$0.sorted{$0.characters.count < $1.characters.count}}
```
