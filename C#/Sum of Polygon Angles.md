## Sum of Polygon Angles

Given an n-sided regular polygon n, return the total sum of internal angles (in degrees).
```c#
Examples
SumPolygon(3) ➞ 180

SumPolygon(4) ➞ 360

SumPolygon(6) ➞ 720
```
### 🥬 My Code
```c#
class Program {public static int SumPolygon(int n)=> (n - 2) * 180; }
```
