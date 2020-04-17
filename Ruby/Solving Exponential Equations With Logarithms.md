## Solving Exponential Equations With Logarithms

Create a function that takes a number a and finds the missing exponent x so that a when raised to the power of x is equal to b.
```ruby
Examples
solve_for_exp(4, 1024) ➞ 5

solve_for_exp(2, 1024) ➞ 10

solve_for_exp(9, 3486784401) ➞ 10
```
### :gem: My Code
```ruby
def solve_for_exp(a, b)
 Math.log(b,a).round
end
```
