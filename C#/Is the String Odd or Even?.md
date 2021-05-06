## Is the String Odd or Even?

Given a string, return true if its length is even or false if the length is odd.
```c#
Examples
oddOrEven("apples") ➞ true
// The word "apples" has 6 characters.
// 6 is an even number, so the program outputs true.

oddOrEven("pears") ➞ false
// "pears" has 5 letters, and 5 is odd.
// Therefore the program outputs false.

oddOrEven("cherry") ➞ true
```
### 🌴 My Code
```c#
class Program {public static bool oddOrEven(string w) => w.Length % 2 == 0;}
```
