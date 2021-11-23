## Vowel Replacer

Create a function that replaces all the vowels in a string with a specified character.
```
Examples
replaceVowels("the aardvark", "#") ➞ "th# ##rdv#rk"

replaceVowels("minnie mouse", "?") ➞ "m?nn?? m??s?"

replaceVowels("shakespeare", "*") ➞ "sh*k*sp**r*"
```
### 💱  My Code
```swift
let replaceVowels:(String, String) -> String = {$0.replacingOccurrences(of: "[aeiou]", with: $1, options: .regularExpression)}
```
