## Not Not Not True

Something which is not true is false, but something which is not not true is true! Create a function where given $n number of "not", evaluate whether it's true or false.
```php
Examples
notNotNot(1, true) ➞ false
// Not true

notNotNot(2, false) ➞ false
// Not not false

notNotNot(6, true) ➞ true
// Not not not not not not true
```
### 🪢 My Code
```php
function notNotNot($n,$b) {
  return $n % 2 ? !$b : $b;
}
```
