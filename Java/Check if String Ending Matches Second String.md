## Check if String Ending Matches Second String

Create a function that takes two strings and returns true if the first string ends with the second string; otherwise return false.
```java
Examples
checkEnding("abc", "bc") ➞ true

checkEnding("abc", "d") ➞ false

checkEnding("samurai", "zi") ➞ false

checkEnding("feminine", "nine") ➞ true

checkEnding("convention", "tio") ➞ false
```
### :coffee: My Code
```java
public class Challenge {
  public static boolean checkEnding(String s1, String s2) {
    return s1.endsWith(s2);
  }
}
```
