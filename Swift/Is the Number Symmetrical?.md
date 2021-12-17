## Is the Number Symmetrical?

Create a function that takes a number as an argument and returns true or false depending on whether the number is symmetrical or not. A number is symmetrical when it is the same as its reverse.
```
Examples
isSymmetrical(7227) ➞ true

isSymmetrical(12567) ➞ false

isSymmetrical(44444444) ➞ true

isSymmetrical(9939) ➞ false

isSymmetrical(1112111) ➞ true
```
### ✒️  My Code
```swift
//using math
func isSymmetrical(_ n: Int) -> Bool {
 var num = n
    var r = 0
    while num > 0 {
        let a = num % 10
        r = r * 10 + a
        num = num / 10
    }
    return n == r    
}

//alternate solution
let isSymmetrical = {(n:Int) in	String("\(n)".characters.reversed()) == "\(n)"}
```
