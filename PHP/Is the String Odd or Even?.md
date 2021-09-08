## Is the String Odd or Even?

Given a string, return true if its length is even or false if the length is odd.
```php
Examples
oddOrEven("apples") ➞ true
// The word "apples" has 6 characters.
// 6 is an even number, so the program outputs true.

oddOrEven("pears") ➞ false
// "pears" has 5 letters, and 5 is odd.
// Therefore the program outputs false.

oddOrEven("cherry") ➞ true
```
### 🌵 My Code
```php
function oddOrEven($w) {
  return strlen($w) % 2 == 0;
}
```
