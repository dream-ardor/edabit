## Inches to Feet

Create a function that accepts a measurement value in inches and returns the equivalent of the measurement value in feet.
```php
Examples
inches_to_feet(324) ➞ 27

inches_to_feet(12) ➞ 1

inches_to_feet(36) ➞ 3

Notes:
If inches are under 12, return 0.
```
### :leaves: My Code
```php
function inches_to_feet($i) {
  return $i > 11 ? $i/12 : 0;
}
```
