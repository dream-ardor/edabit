## Let's Fuel Up!

A vehicle needs 10 times the amount of fuel than the distance it travels. However, it must always carry a minimum of 100 fuel before setting off.

Create a function which calculates the amount of fuel it needs, given the distance.
```java
Examples
calculateFuel(15) ➞ 150

calculateFuel(23.5) ➞ 235

calculateFuel(3) ➞ 100
```
  
 ### ☕ My Code
 ```java
 class FuelUp {
  static double calculateFuel(double n) {
   return n < 10 ? 100 : n * 10;
	}
}
  ```
