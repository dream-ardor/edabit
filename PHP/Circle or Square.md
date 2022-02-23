## Circle or Square

Given the radius of a circle and the area of a square, return true if the circumference of the circle is greater than the square's perimeter and false if the square's perimeter is greater than the circumference of the circle.
```php
Examples
circleOrSquare(16, 625) ➞ true

circleOrSquare(5, 100) ➞ false

circleOrSquare(8, 144) ➞ true
```
### 🔵  My Code  🟦
```php
function circleOrSquare($r,$a) {
  return $r * 1.57 > $a ** 0.5;
}	
```
