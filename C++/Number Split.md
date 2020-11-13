## Number Split

Given a number, return an array containing the two halves of the number. If the number is odd, make the rightmost number higher.
```c++
Examples
numberSplit(4) ➞ [2, 2]

numberSplit(10) ➞ [5, 5]

numberSplit(11) ➞ [5, 6]

numberSplit(-9) ➞ [-5, -4]

Notes:
All numbers will be integers.
You can expect negative numbers too.
```
### :palm_tree: My Code
```c++
#include <cmath>
#define numberSplit(n)std::vector<int>{(int)floor(n/2.f),(int)ceil(n/2.f)}
```
