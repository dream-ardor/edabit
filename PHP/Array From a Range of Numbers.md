## Array From a Range of Numbers

Create a function that returns an array of all the integers between two given numbers $start and $end.
```php
Examples
rangeOfNum(2, 4) ➞ [3]

rangeOfNum(5, 9) ➞ [6, 7, 8]

rangeOfNum(2, 11) ➞ [3, 4, 5, 6, 7, 8, 9, 10]

Notes:
$start will always be <= $end.
$start and $end are NOT included in the final array.
If $start == $end, return an empty array.
```
### 📙 My Code
```php
function rangeOfNum($s,$e) {
  return $s != $e ? range($s + 1, $e - 1) : [] ;
}

//alternate solution
function rangeOfNum($s,$e) {
   $a = [];
  for ($i = $s + 1; $i <= $e - 1; ++$i) {
   $a[] = $i;};
  return $a;
}
```
