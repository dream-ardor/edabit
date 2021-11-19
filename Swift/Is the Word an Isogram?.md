## Is the Word an Isogram?

An isogram is a word that has no duplicate letters. Create a function that takes a string and returns either true or false depending on whether or not it's an "isogram".
```
Examples
isIsogram("Algorism") ➞ true

isIsogram("PasSword") ➞ false
// Not case sensitive.

isIsogram("Consecutive") ➞ false
```
### 🏺 My Code
```swift
let isIsogram:(String) -> Bool = {Set($0.lowercased().characters).count == $0.characters.count}
```
