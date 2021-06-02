## How Much is True?

Create a function which returns the number of true values there are in an array.
```c#
Examples
CountTrue([true, false, false, true, false]) ➞ 2

CountTrue([false, false, false, false]) ➞ 0

CountTrue([]) ➞ 0
```
### 🌻 My Code
```c#
using System.Linq;
class Program {public static int CountTrue(bool[] a) => a.Count(x => x);}
```
