## Is it Time for Milk and Cookies?

Christmas Eve is almost upon us, so naturally we need to prepare some milk and cookies for Santa! Create a function that accepts a (year, month, day) of date and returns true if it's Christmas Eve (December 24th) and false otherwise. Keep in mind that month of Date is 0 based, meaning December is the 11th month while January is 0.
```c++
Examples
timeForMilkAndCookies(2013, 11, 24) ➞ true

timeForMilkAndCookies(2013, 0, 23) ➞ false

timeForMilkAndCookies(3000, 11, 24) ➞ true

Notes:
Dates in C++ are zero based (see Resources).
All test cases contain valid dates.
```
### :leaves: My Code
```c++
#define timeForMilkAndCookies(y,m,d) m==11 && d==24
```
