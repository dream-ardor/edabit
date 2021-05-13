## Return a String as an Integer

Create a function that takes a string and returns it as an integer.
```c#
Examples
StringInt("6") ➞ 6

StringInt("1000") ➞ 1000

StringInt("12") ➞ 12
```
### 🌴 My Code
```c#
class Program {public static int StringInt(string t)=> int.Parse(t);}


//alternate solution
public class Program 
{
  public static int StringInt(string t) {
   int n = 0;
    foreach (var c in t)
     n = (n << 1) + (n << 3) + (c - '0');
   return n;
}
}
```
