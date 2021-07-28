## Find the Bug: Checking Even Numbers

Create a function that takes in an array and returns true if all its values are even, and false otherwise.

Not a big deal, your friend says. He writes the following code:
```swift
func checkAllEven(_ arr:[Int]) -> Bool {
  return arr.filter{$0%2==0}.count != 0
}

Fix the code above so that all tests pass:

Examples
checkAllEven([1, 2, 3, 4]) ➞ false

checkAllEven([2, 4, 6]) ➞ true

checkAllEven([5, 6, 8, 10]) ➞ false

checkAllEven([-2, 2, -2, 2]) ➞ true
```
### 2️⃣ My Code
```swift
let checkAllEven: ([Int]) -> Bool = {$0.filter{$0 % 2 > 0}.count < 1}
```
