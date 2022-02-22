## Rotate Max Number

Create a function which takes a number and returns the maximum value by rearranging its digits.
```php
Examples
rotateMaxNumber(123) ➞ 321

rotateMaxNumber("001") ➞ 100

rotateMaxNumber(999) ➞ 999
```
### 🚨 My Code
```php
function rotateMaxNumber($n) {
  $a = str_split($n);
  return rsort($a);
}

```
