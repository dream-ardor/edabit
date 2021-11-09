## Negate the Array of Numbers

Given an array of numbers, negate all elements contained within.

Negating a positive value -+n will return -n, because all +'s are removed.
Negating a negative value --n will return n, because the first - turns the second minus into a +.
```
Examples

negate([1, 2, 3, 4]) ➞ [-1, -2, -3, -4]

negate([-1, 2, -3, 4]) ➞ [1, -2, 3, -4]

negate([]) ➞ []
```
### ❎ My Code
```php
function negate($a) {
  return array_map(function($b) { return $b * -1; }, $a);
}
```
