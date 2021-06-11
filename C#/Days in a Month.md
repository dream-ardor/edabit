## Days in a Month

Create a function that takes the month and year (as integers) and returns the number of days in that month.
```c#
Examples
Days(2, 2018) ➞ 28

Days(4, 654) ➞ 30

Days(2, 200) ➞ 29

Days(2, 1000) ➞ 29
```

### 📆 My Code
```c#
using System;
public class Program {public static int Days(int m, int y) => DateTime.DaysInMonth(y, m);}
```
