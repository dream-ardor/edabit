## Amazing Edabit!

Create a function that takes a string and changes the word amazing to not amazing. Return the string without any change if the word edabit is part of the string.
```swift
Examples
amazingEdabit("edabit is amazing.") ➞ "edabit is amazing."

amazingEdabit("Mubashir is amazing.") ➞ "Mubashir is not amazing."

amazingEdabit("Infinity is amazing.") ➞ "Infinity is not amazing."
```

### 🏋️ My Code
```swift
let amazingEdabit:(String) -> String = {$0.contains("edabit") ? $0 : $0.replacingOccurrences(of:"is", with:"is not")}
```
