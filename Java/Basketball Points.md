## Basketball Points

You are counting points for a basketball game, given the amount of 2-pointers scored and 3-pointers scored, find the final points for the team and return that value.
```java
Examples
points(13, 12) ➞ 62

points(17, 12) ➞ 70

points(38, 8) ➞ 100
```
### :basketball: My Code
```java
public class BasketballPoints { 
  public static int points(int a, int b) {
   return a*2 + b*3;
  }
}
```
