## Count the Arguments

Create a method that returns the number of arguments it was called with.
```c#
Examples
NumArgs() ➞ 0

NumArgs("foo") ➞ 1

NumArgs("foo", "bar") ➞ 2

NumArgs(true, false) ➞ 2

NumArgs({}) ➞ 1
```
### 🌲 My Code
```c#
class Program {public static int NumArgs(params object[]p) => p.Length;}
```
