## FizzBuzz Interview Question

Create a function that takes a number as an argument and returns "Fizz", "Buzz" or "FizzBuzz".
```
If the number is a multiple of 3 the output should be "Fizz".
If the number given is a multiple of 5, the output should be "Buzz".
If the number given is a multiple of both 3 and 5, the output should be "FizzBuzz".
If the number is not a multiple of either 3 or 5, the number should be output on its own as shown in the examples below.
```
```js
Examples
FizzBuzz(3) ➞ "Fizz"

FizzBuzz(5) ➞ "Buzz"

FizzBuzz(15) ➞ "FizzBuzz"

FizzBuzz(4) ➞ "4"
```
### :cloud_with_rain: My Code
```js
const FizzBuzz = n => 
 n %3 ==0 && n % 5==0 ? "FizzBuzz": n % 3 == 0 ? "Fizz" :
 n % 5 == 0 ? "Buzz" : String(n);
```
