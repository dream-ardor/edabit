## Recreating the abs() Function

The abs() function returns the absolute value of a number. This means it returns a number's positive value. You can think of it as the distance away from zero.

Create a function that recreates this functionality.
```swift
Examples
absolute(-5) ➞ 5

absolute(-3.14) ➞ 3.14

absolute(250) ➞ 250
```
### 0️⃣ My Code
```swift
let absolute = {$0 > 1 ? $0 : $0 * (-1)}
```
