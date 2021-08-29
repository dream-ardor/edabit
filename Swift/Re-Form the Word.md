## Re-Form the Word

A word has been split into a left part and a right part. Re-form the word by adding both halves together, changing the first character to an uppercase letter.
```swift
Examples
getWord("seas", "onal") ➞ "Seasonal"

getWord("comp", "lete") ➞ "Complete"

getWord("lang", "uage") ➞ "Language"
```
### ☀️ My Code
```swift

let getWord: (String,String) -> String = {($0+$1).capitalized}

or 

let getWord : (String, String) -> String = {"\($0)\($1)".capitalized}
```
