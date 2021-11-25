## Which Function Returns the Larger Number?

Your function will be passed two functions, f and g, that don't take any parameters. Your function has to call them, and return a string which indicates which function returned the larger number.
```
If f returns the larger number, return the string f.
If g returns the larger number, return the string g.
If the functions return the same number, return the string neither.

Examples
larger({5}, {10}) ➞ "g"

larger({25}, {25}) ➞ "neither"

larger({505050}, {5050}) ➞ "f"
```
### ➰ My Code
```swift
func larger(_ f: () -> Int, _ g: () -> Int) -> String {
  return f() > g() ? "f" : f() < g() ? "g" : "neither"
}
```
