## Power Calculator

Create a function that takes voltage and current and returns the calculated power.
```swift
Examples
circuitPower(230, 10) ➞ 2300

circuitPower(110, 3) ➞ 330

circuitPower(480, 20) ➞ 9600
```
### :leaves: My Code
```swift
let circuitPower = {(v:Int, c:Int ) in v * c}

//alternate solutions
let circuitPower: (Int,Int) -> Int = {$0*$1}

func circuitPower(_ v: Int, _ c: Int) -> Int {
	return v * c
}
```
