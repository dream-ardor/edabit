## Find the Smallest Number in an Array

Create a function that takes an array of numbers and returns the smallest number in the set.
```c#
Examples
FindSmallestNum([34, 15, 88, 2]) ➞ 2

FindSmallestNum([34, -345, -1, 100]) ➞ -345

FindSmallestNum([-76, 1.345, 1, 0]) ➞ -76

FindSmallestNum([0.4356, 0.8795, 0.5435, -0.9999]) ➞ -0.9999

FindSmallestNum([7, 7, 7]) ➞ 7
```
### 🌴 My Code
```c#
using System.Linq;
class Program {public static double FindSmallestNum(double[] a)=> a.Min();}
```
