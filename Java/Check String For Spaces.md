## Check String for Spaces
Create a function that returns true if a string contains any spaces.
```java
Examples
hasSpaces("hello") ➞ false

hasSpaces("hello, world") ➞ true

hasSpaces(" ") ➞ true

hasSpaces("") ➞ false

hasSpaces(",./!@#") ➞ false
```
### :hotsprings:My Code
```java
public class Challenge {
	public static boolean hasSpaces(String str) {
		return str.contains(" ");
	}
}
```
