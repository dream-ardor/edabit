## Concatenate First and Last Name into One String

Given two strings, firstName and lastName, return a single string in the format "last, first".
```c#
Examples
ConcatName("First", "Last") ➞ "Last, First"

ConcatName("John", "Doe") ➞ "Doe, John"

ConcatName("Mary", "Jane") ➞ "Jane, Mary"
```
### 🌳 My Code
```c#
class Program {public static string ConcatName(string f, string l) => l + ", " + f;}
```
