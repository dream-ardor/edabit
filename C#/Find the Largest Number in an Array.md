## Find the Largest Number in an Array

Create a function that takes an array of numbers. Return the largest number in the array.
```c#
Examples
findLargestNum([4, 5, 1, 3]) ➞ 5

findLargestNum([300, 200, 600, 150]) ➞ 600

findLargestNum([1000, 1001, 857, 1]) ➞ 1001
```
### 🌿 My Code
```c#
using System.Linq;
class Program{ public static int FindLargestNum(int[] a) => a.Max();}
```
