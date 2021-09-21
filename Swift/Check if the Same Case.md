## Check if the Same Case

Create a function that returns true if an input string contains only uppercase or only lowercase letters.
```swift
Examples

sameCase("hello") ➞ true

sameCase("HELLO") ➞ true

sameCase("Hello") ➞ false

sameCase("ketcHUp") ➞ false
```
### 📘 My Code
```swift
let sameCase = {$0 == $0.uppercased() || $0 == $0.lowercased()}
```
