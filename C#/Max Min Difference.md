## Max Min Difference

Given an array of integers, return the difference between the largest and smallest integers on the array .
```c#
Examples
Diff([10, 15, 20, 2, 10, 6]) ➞ 18
// 20 - 2 = 18

Diff([-3, 4, -9, -1, -2, 15]) ➞ 24
// 15 - (-9) = 24

Diff([4, 17, 12, 2, 10, 2]) ➞ 15
```
### 🌳 My Code
```c#
using System.Linq;
public class Program
{ public static int Diff(int[] a){
   return a.Max() - a.Min();}
}
```
