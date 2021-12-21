## Maximum Weight Allowed

Create a function that returns true if the combined weight of a car $car and the weight of the passengers $p in the car is less than the maximum weight $maxWeight the car is allowed to carry. Otherwise, return false. The weight of the car and the weight of the passengers are given in pounds. The maximum weight is given in kilograms.
```
Examples
weightAllowed(3000, [150, 201, 75, 88, 195], 1700) ➞ true

weightAllowed(3200, [220, 101, 115, 228, 15], 1700) ➞ false

weightAllowed(2900, [225, 171, 300, 274, 191], 1850) ➞ true
```
### 🚙 My Code
```php
function weightAllowed($c, $p, $m) {
  return $c + array_sum($p) < $m * 2.2;
}
```
