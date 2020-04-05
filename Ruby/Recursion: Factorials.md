## Recursion: Factorials

Write a function that calculates the factorial of a number recursively.
```ruby
Examples
factorial(5) ➞ 120

factorial(3) ➞ 6

factorial(1) ➞ 1

factorial(0) ➞ 1
```
### :gem: My Code
```ruby
def factorial(n)
 n < 2 ? 1 : n * factorial(n-1)
end
```
