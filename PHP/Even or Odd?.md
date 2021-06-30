## Even or Odd?
Given an array of integers, determine whether the sum of its elements is even or odd.

The return value should be a string ("odd" or "even").

If the input array is empty, consider it as an array with a zero ([0]).
```
Examples
evenOrOdd([0]) ➞ "even"

evenOrOdd([1]) ➞ "odd"

evenOrOdd([]) ➞ "even"

evenOrOdd([0, 1, 5]) ➞ "even"
```
### 🌴 My Code
```php
function evenOrOdd($a) {
  return array_sum($a) % 2 ? "odd" : "even";
}
```
