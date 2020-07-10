## Recursion: Fibonacci Numbers

Fibonacci numbers are created in the following way:
```ruby
F(0) = 0
F(1) = 1
...
F(n) = F(n-2) + F(n-1)
```
Write a function that calculates the nth Fibonacci number.
```ruby
Examples
fib(0) ➞ 0

fib(1) ➞ 1

fib(2) ➞ 1

fib(8) ➞ 21
```
### :gem: My Code
```ruby
def fib(n)
  n < 2 ? n : fib(n-1) + fib(n-2)
end
```
