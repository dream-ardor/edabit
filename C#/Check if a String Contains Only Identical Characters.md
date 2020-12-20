## Check if a String Contains only Identical Characters

Write a function that returns true if all characters in a string are identical and false otherwise.
```c#
Examples

isIdentical("aaaaaa") ➞ true

isIdentical("aabaaa") ➞ false

isIdentical("ccccca") ➞ false

isIdentical("kk") ➞ true
```
### :evergreen_tree:	My Code
```c#
using System.Linq;
public class Program
{public static bool isIdentical(string s) => s.Distinct().Count() == 1;}


//alternate solutions
using System.Linq;
public class Program
{
  public static bool isIdentical(string s) => s.All(c => c == s[0]);
}

public class Program
{
  public static bool isIdentical(string str) => str.Trim(str[0]) == "";
}

```
