## Check if String Ending Matches Second String

Create a function that takes two strings and returns true if the first string ends with the second string; otherwise return false.
```c#
Examples
CheckEnding("abc", "bc") ➞ true

CheckEnding("abc", "d") ➞ false

CheckEnding("samurai", "zi") ➞ false

CheckEnding("feminine", "nine") ➞ true

CheckEnding("convention", "tio") ➞ false
```
### 🌿 My Code
```c#
class Program {public static bool CheckEnding(string a,string b) => a.EndsWith(b);}
```
