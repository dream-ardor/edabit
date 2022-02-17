## Cube the Square Root

Create a function that takes a number as an argument and returns the square root of that number cubed.
```java
Examples
cubeSquareRoot (81) ➞ 729

cubeSquareRoot (1646089) ➞ 2111932187

cubeSquareRoot (695556) ➞ 580093704
 ```
 ### ♨️   My Code
 ```java
public class Challenge {
  public static int cubeSquareRoot(int n) {
    return (int)Math.pow(n, 1.5);
  }
}
```
