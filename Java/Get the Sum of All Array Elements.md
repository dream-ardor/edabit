## Get the Sum of All Array Elements

Create a function that takes an array and returns the sum of all numbers in the array.
```java
Examples
sum([2, 7, 4]) ➞ 13

sum([45, 3, 0]) ➞ 48

sum([-2, 84, 23]) ➞ 105
```
### ☕  My Code
```java
public class Program {
  public static int arraySum(int[] a) {
  int b = 0;
  for (int i = 0; i < a.length; b += a[i++]);
  return b;
  }
}
```
