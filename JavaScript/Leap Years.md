## Leap Years

A leap year has one day added to February for being synchronized with the seasonal year. A leap year appears with a regular frequency, which is determined by the rule below:

The year is exactly divisible by 400, or exactly divisible by 4 and not exactly divisible by 100.
Given a year you must implement a function that returns true if it's a leap year, or false if it's not.
```js
Examples
isLeap(2020) ➞ true
// Exactly divided by 4 and not by 100.

isLeap(1800) ➞ false
// Exactly divided by 4, but is also exactly divided by 100.

isLeap(2000) ➞ true
// Exactly divided by 400.

isLeap(2019) ➞ false
// It can't be exactly divided by 400 or by 4.
```
### :jack_o_lantern: My Code
```js
const isLeap = y => y % 400 == 0 || y % 4 == 0 && y % 100 != 0; 

```
