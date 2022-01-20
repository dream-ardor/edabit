## Is the Number Symmetrical?

Create a function that takes a number as an argument and returns true or false depending on whether the number is symmetrical or not. A number is symmetrical when it is the same as its reverse.
```php
Examples
isSymmetrical(7227) ➞ true

isSymmetrical(12567) ➞ false

isSymmetrical(44444444) ➞ true

isSymmetrical(9939) ➞ false

isSymmetrical(1112111) ➞ true
```
### 🉑 My Code
```php
function isSymmetrical($n) {
  return $n == strrev(strval($n));
}
```
