## Recreating the abs() Function

The Math.Abs() function returns the absolute value of a number. This means that it returns a number's positive value. You can think of it as the distance away from zero.

Create a function that recreates this functionality.
```c# 
Examples
absolute(-3) ➞ 3

absolute(250) ➞ 250

Notes
Tests will only include valid numbers.
Don't use the Math.Abs() function (it will defeat the purpose of the challenge).
```
### 🍁 My Code
```c#
class Program {public static int absolute(int n)=> n > 0 ? n : -n;}
```
