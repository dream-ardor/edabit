## Smaller String Number

Create a function that returns the smaller number.
```php
Examples
smallerNum("21", "44") ➞ "21"

smallerNum("1500", "1") ➞ "1"

smallerNum("5", "5") ➞ "5"
```
### ⛈️ My Code
```php
use function min as smallerNum;


//alternate solution
function smallerNum($a, $b) {
  return min($a, $b);
}
```
