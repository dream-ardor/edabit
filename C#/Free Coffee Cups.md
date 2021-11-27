## Free Coffee Cups

For each of the 6 coffee cups I buy, I get a 7th cup free. In total, I get 7 cups. Create a function that takes n cups bought and return the total number of cups I would get.
```c#
Examples

TotalCups(6) ➞ 7

TotalCups(12) ➞ 14

TotalCups(213) ➞ 248
```
### ☕ My Code
```c#
class Program {public static int TotalCups(int n) => n + (n/6);}
```
