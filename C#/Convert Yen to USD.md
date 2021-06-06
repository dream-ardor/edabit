## Convert Yen to USD

Create a function that can turn Yen (Japanese dollar) to USD (American dollar).
```c#
Examples
YenToUsd(1) ➞ 0.01

YenToUsd(500) ➞ 4.65

YenToUsd(649) ➞ 6.04
```
### 💴 My Code
```c#
using System;
class Program {public static double YenToUsd(int y) => Math.Round(y / 107.5, 2);}
```
