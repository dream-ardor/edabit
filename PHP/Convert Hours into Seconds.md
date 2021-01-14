## Convert Hours into Seconds

Write a function that converts hours into seconds.
```php
Examples
howManySeconds(2) ➞ 7200

howManySeconds(10) ➞ 36000

howManySeconds(24) ➞ 86400

Notes:

60 seconds in a minute, 60 minutes in an hour
Don't forget to return your answer.
```
### :leaves: My Code
```php
function howManySeconds($h) {
  return $h * 3600;
}
```
