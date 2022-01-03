## End Corona!

Create a function that takes the number of activeCases, daily average recovered cases and daily average newCases and calculates the number of days it will take to reach zero cases.
```
Examples

endCorona(4000, 2000, 77000) ➞ 39

endCorona(3000, 2000, 50699) ➞ 51

endCorona(30000, 25000, 390205) ➞ 79
```
### 💥 My Code
```c++
#define endCorona(a,b,c) c / (a-b)+1
```
