## Find the Discount

Create a function that takes two arguments: the original price and the discount percentage as integers and returns the final price after the discount.

```php
Examples

discount(1500, 50) ➞ 750

discount(89, 20) ➞ 71.2

discount(100, 75) ➞ 25
```

### 💲 My Code
```php
function discount($p,$d) {
  return $p * (100 - $d)/100;
}
```
