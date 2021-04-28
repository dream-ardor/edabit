## Is it Time for Milk and Cookies?

Christmas Eve is almost upon us, so naturally we need to prepare some milk and cookies for Santa! Create a function that accepts year, month and day as integers and returns true if it's Christmas Eve (December 24th) and false otherwise.
```c#

Examples
Date( 2013, 12, 24 ) ➞ true

Date( 2013, 0, 23 ) ➞ false

Date( 3000, 12, 24 ) ➞ true
```
### 🥛 🍪 My Code
```c#
class Program {public static bool TimeForMilkAndCookies(int y,int m,int d) => m + d == 36;}
```
