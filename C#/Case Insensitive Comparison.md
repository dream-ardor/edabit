## Case Insensitive Comparison

Write a function that validates whether two strings are identical. Make it case insensitive.
```c#
Examples
match("hello", "hELLo") ➞ true

match("motive", "emotive") ➞ false

match("venom", "VENOM") ➞ true

match("mask", "mAskinG") ➞ false
```
### 🥀 My Code
```c#
public class Program
{public static bool match(string a, string b) => a.ToLower() == b.ToLower();}

//alternative solution
using System;
class Program {public static bool match(string a, string b) => a.Equals(b, StringComparison.CurrentCultureIgnoreCase);}
```
