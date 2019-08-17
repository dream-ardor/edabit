## Return the Factorial
Create a function that takes an integer and returns the factorial of that integer. That is, the integer multiplied by all positive lower integers.
```ruby
Examples
factorial(3) ➞ 6

factorial(5) ➞ 120

factorial(13) ➞ 6227020800
```
### :gem:My Code
```ruby
def factorial(i)
  (1..i).inject(:*)
end
```
