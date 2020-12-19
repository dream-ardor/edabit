## Find the Smallest and Biggest Numbers

Create a function that takes an array of numbers and return both the minimum and maximum numbers, in that order.
```c#
Examples
FindMinMax([1, 2, 3, 4, 5]) ➞ [1, 5]

FindMinMax([2334454, 5]) ➞ [5, 2334454]

FindMinMax([1]) ➞ [1, 1]
```
### :maple_leaf: My Code
```c#
using System;
using System.Linq;
public class Program 
{public static double[] FindMinMax(double[] v) =>
  new [] {v.Min(), v.Max()};   
}
```
