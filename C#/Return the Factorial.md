## Return the Factorial

Create a function that takes an integer and returns the factorial of that integer. That is, the integer multiplied by all positive lower integers.
```
Examples

Factorial(3) ➞ 6

Factorial(5) ➞ 120

Factorial(13) ➞ 6227020800
```
### :leaves: My Code
```c#
class Program
{public static int Factorial(int n) => n < 2 ? n: n * Factorial(n-1);}


//alternate
public class Program
{public static int Factorial(int n)
  {if (n == 1)
   return 1;
    else
     return n * Factorial(n - 1);
   }
}
```
