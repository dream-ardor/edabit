## Integer Digits Count

Create a function that counts the integer's number of digits.
```swift
Examples
count(318) ➞ 3
 
count(-92563) ➞ 5
 
count(4666) ➞ 4

count(-314890) ➞ 6

count(654321) ➞ 6

count(638476) ➞ 6
```
### 🖥️ My Code
```swift
let count = {String(abs($0)).characters.count}
```
