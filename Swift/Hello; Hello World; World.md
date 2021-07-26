## Hello; Hello World; World

Write a function that takes an integer and:
```
If the number is a multiple of 3, return "Hello".
If the number is a multiple of 5, return "World".
If the number is a multiple of both 3 and 5, return "Hello World".

Examples
helloWorld(3) ➞ "Hello"

helloWorld(5) ➞ "World"

helloWorld(15) ➞ "Hello World"
```
### 🌏 My Code
```swift
let helloWorld = {$0 % 15 == 0 ? "Hello World" : $0 % 5 == 0 ? "World" : "Hello"}
```
