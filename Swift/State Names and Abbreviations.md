## State Names and Abbreviations

Create a function that filters out an array of state names into two categories based on the second parameter.
```
Abbreviations abb
Full names full

Examples
filterStateNames(["Arizona", "CA", "NY", "Nevada"], "abb")
➞ ["CA", "NY"]

filterStateNames(["Arizona", "CA", "NY", "Nevada"], "full")
➞ ["Arizona", "Nevada"]

filterStateNames(["MT", "NJ", "TX", "ID", "IL"], "abb")
➞ ["MT", "NJ", "TX", "ID", "IL"]

filterStateNames(["MT", "NJ", "TX", "ID", "IL"], "full")
➞ []
```
### 🌎  My Code
```swift
let filterStateNames:([String],String) -> [String] = {$1 == "full" ? $0.filter{$0.characters.count > 2 } : $0.filter{$0.characters.count == 2}}
```
