## String to Integer and Vice Versa
```
Write two functions:

toInt() : A function to convert a string to an integer.
toStr() : A function to convert an integer to a string.

Examples
toInt("77") ➞ 77

toInt("532") ➞ 532

toStr(77) ➞ "77"

toStr(532) ➞ "532"
```
### 🍃 My Code
```c#
class Program
{public static int toInt(string s)=> int.Parse(s);
 public static string toStr(int n)=> n.ToString();
}
```
