## Count Instances of a Character in a String

Create a function that takes a character and a string as arguments and returns the number of times the character is found in the string.
```c#
Examples
CharCount('a', "edabit") ➞ 1

CharCount('c', "Chamber of secrets") ➞ 1

CharCount('b', "big fat bubble") ➞ 4
```
### 🔤 My Code
```c#
using System.Linq;
class Program {public static int CharCount(char a,string s)=> s.Count(b => b == a);}

//alternative solution
public class Program {public static int CharCount(char c, string s)=> s.Split(c).Length - 1;}
```
