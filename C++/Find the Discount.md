## Find the Discount

Create a function that takes two arguments: the original price and the discount percentage as integers and returns the final price after the discount.

Alternative Text
```
Examples

dis(1500, 50) ➞ 750

dis(89, 20) ➞ 71.2

dis(100, 75) ➞ 25
```
### 🪙  My Code
```c++
#define dis(p, d)p * (100.0 - d) / 100.0
```
