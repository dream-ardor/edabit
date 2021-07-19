Burrrrrrrp

Create a function that returns the string "Burp" with the amount of "r's" determined by the input parameters of the function.
```php
Examples
longBurp(3) ➞ "Burrrp"

longBurp(5) ➞ "Burrrrrp"

longBurp(9) ➞ "Burrrrrrrrrp"
```
### ⛈️ My Code
```php
function longBurp($n) {
  return "Bu" . str_repeat("r",$n) . "p";
}
```
