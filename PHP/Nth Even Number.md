## Nth Even Number

Create a function that takes a number n and returns the nth even number.
```php
Examples
nth_even(1) ➞ 0
# 0 is first even number

nth_even(2) ➞ 2
# 2 is second even number

nth_even(100) ➞ 198
```
### 8️⃣ My Code
```php
function nthEven($n) {
  return $n * 2 - 2;
}
```
