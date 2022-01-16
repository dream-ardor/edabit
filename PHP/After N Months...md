## After N Months...

Create a function that takes in $year and $months as input, then return what year it would be after n-months have elapsed.
```php
Examples
afterNMonths(2020, 24) ➞ 2022

afterNMonths(1832, 2) ➞ 1832

afterNMonths(1444, 60) ➞ 1449

Notes

Assume that adding 12 months will always increment the year by 1.
If no value is given for $year or $months, return "year missing" or "month missing".
At least one value will be present.
```
### 🗓️ My Code
```php
function afterNMonths($y, $m) {
  return $y ? $m ? $y + $m / 12 || 0 :"month missing":"year missing";
}
```
