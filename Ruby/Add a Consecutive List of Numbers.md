## Add a Consecutive List of Numbers

Write a function that takes the last number of a consecutive list of numbers and returns the total of all numbers up to and including it.
```ruby
Examples
add_up_to(3) ➞ 6
# 1 + 2 + 3 = 6

add_up_to(10) ➞ 55
# 1 + 2 + 3 + ... + 10 = 55

add_up_to(7) ➞ 28
# 1 + 2 + 3 + ... + 7 = 28
```
### :gem: My Code
```ruby
def add_up_to(n)
  [*1..n].reduce(0,:+)
end
```
