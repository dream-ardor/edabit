## Is It a Triangle?

Create a function that takes three numbers as arguments and returns true if it's a triangle and false if not.
```
Examples
isTriangle(2, 3, 4) ➞ true

isTriangle(3, 4, 5) ➞ true

isTriangle(4, 3, 8) ➞ false
```
### 🔺  My Code
```c++
#define isTriangle(a,b,c) a + b > c && b + c > a && c + a > b
```
