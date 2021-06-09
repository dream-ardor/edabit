## Convert Hours and Minutes into Seconds

Write a function that takes two integers (hours, minutes), converts them to seconds, and adds them.
```java
Examples
convert(1, 3) ➞ 3780

convert(2, 0) ➞ 7200

convert(0, 0) ➞ 0
```
### ⏰ My Code
```java
public class Challenge {
  public static int convert(int h, int m) {
    return h * 3600 + m * 60;
  }
}
```
