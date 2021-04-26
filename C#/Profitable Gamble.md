## Profitable Gamble

Create a function that takes three arguments prob, prize, pay and returns true if prob * prize > pay; otherwise return false.

To illustrate:
```c#
ProfitableGamble(0.2, 50, 9)
... should yield true, since the net profit is 1 (0.2 * 50 - 9), and 1 > 0.

Examples
ProfitableGamble(0.2, 50, 9) ➞ true

ProfitableGamble(0.9, 1, 2) ➞ false

ProfitableGamble(0.9, 3, 2) ➞ true
```
### 🌴 My Code
```c#
class Program {public static bool ProfitableGamble(double a,int b,double c) => a * b > c;}
```
