## Free Coffee Cups

For each of the 6 coffee cups I buy, I get a 7th cup free. In total, I get 7 cups. Create a function that takes n cups bought and return as an integer the total number of cups I would get.
```
Examples
totalCups(6) ➞ 7

totalCups(12) ➞ 14

totalCups(213) ➞ 248
```
### ☕  My Code
```c++
#define totalCups(n) n + (n/6)
```
