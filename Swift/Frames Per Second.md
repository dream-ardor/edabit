## Frames Per Second

Create a function that returns the number of frames shown in a given number of minutes for a certain FPS.
```swift
Examples
frames(1, 1) ➞ 60

frames(10, 1) ➞ 600

frames(10, 25) ➞ 15000
```
### 📷 My Code
```swift
let frames = {$0 * $1 * 60}
```
