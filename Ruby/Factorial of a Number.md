## Factorial of a Number

Create a function that receives a non-negative integer and returns the factorial of that number.
```ruby
Examples
fact(0) ➞ 1

fact(1) ➞ 1

fact(3) ➞ 6

fact(6) ➞ 720
```
### :gem: My Code
```ruby
def fact(n)
 (1..n).reduce(1,:*)
end
```
