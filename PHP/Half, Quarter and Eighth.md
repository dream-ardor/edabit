## Half, Quarter and Eighth

Create a function that takes a number and return an array of three numbers: half of the number, quarter of the number and an eighth of the number.
```php
Examples
halfQuarterEighth(6) ➞ [3, 1.5, 0.75]

halfQuarterEighth(22) ➞ [11, 5.5, 2.75]

halfQuarterEighth(25) ➞ [12.5, 6.25, 3.125]
```
### 📊 My Code
```php
function halfQuarterEighth($n) {
  return [$n/2, $n/4, $n/8];
}
```
