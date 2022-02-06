## Return the First and Last Elements in an Array

Create a function that takes an array of values and returns the first and last values in a new array.
```php
Examples
firstLast([5, 10, 15, 20, 25]) ➞ [5, 25]

firstLast(["edabit", 13, null, false, true]) ➞ ["edabit", true]

firstLast([undefined, 4, "6", "hello", null]) ➞ [undefined, null]
```
### 🌓 My Code
```php
function firstLast($a) {
  return [current($a), end($a)];
}
```
