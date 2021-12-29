## Squares and Cubes

Create a function that takes an array of two numbers and checks if the square root of the first number is equal to the cube root of the second number.
```java
Examples

checkSquareAndCube([4, 8]) ➞ true

checkSquareAndCube([16, 48]) ➞ false

checkSquareAndCube([9, 27]) ➞ true
```
### 🧊 My Code
```java
public class Challenge{
  public static boolean squaresAndCubes(int[] a) {
   return Math.sqrt(a[0]) == Math.cbrt(a[1]);
  }
}

//alternate solution
class Challenge{
  public static boolean squaresAndCubes(int[] a) {
   return Math.pow(a[0],1.5)==a[1];
  }
}
```
