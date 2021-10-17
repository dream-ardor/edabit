## Sum Of Polygon Angles

Given an n-sided regular polygon n, return the total sum of internal angles (in degrees).
```java
Examples
sumOfAngles(3) ➞ 180

sumOfAngles(4) ➞ 360

sumOfAngles(6) ➞ 720
```
### ☕ My Code
 ```java
class Polygon { 
static int sumOfAngles(int n) {
  return (n - 2) * 180;
  }
}
 ```
