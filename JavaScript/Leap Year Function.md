## Leap year function ⌚

Write a function that returns true if a year is a leap, otherwise it returns false.

A year is a leap year if it lasts 366 days, instead of 365 in a typical year. That extra day is added to the end of the shorter month, dating as February 29.

To eliminate this error, the Gregorian calendar stipulates that a year that is divisible by 100 (for example, 1900) is a leap year only if it is also divisible by 400. This is because they are divisible by 100 but not by 400. This It is because they are divisible by 100 and 400.

Look at the examples, if you need help look at the resources panel.
```js
Examples
leapYear(1990)➞ false

leapYear(1924)➞ true

leapYear(2021) ➞ false
```
### :calendar: My Code
```js
const leapYear = y => !(y & 3 || y & 15 && !(y % 25));


//alternate solution
const leapYear = y => new Date(y, 1, 29).getDate() == 29;
```
