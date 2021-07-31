## Count Syllables

Create a function that counts the number of syllables a word has. Each syllable is separated with a dash -.
```swift
Examples
numberSyllables("buf-fet") ➞ 2

numberSyllables("beau-ti-ful") ➞ 3

numberSyllables("mon-u-men-tal") ➞ 4

numberSyllables("on-o-mat-o-poe-ia") ➞ 6
```
### 🌄 My Code
```swift
let numberSyllables:(String) -> Int = {$0._split(separator: "-").count}

or

let numberSyllables:(String) -> Int = {$0.components(separatedBy: "-").count}
```
