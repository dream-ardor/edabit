## Nth Star Number

Create a function that takes a positive integer n and returns the nth "star number".

A star number is a centered figurate number a centered hexagram (six-pointed star), such as the one that Chinese checkers is played on.
```ruby
Examples
star_number(2) ➞ 13
# n = 2
# 2nd star number = 13

star_number(3) ➞ 37
# n = 3
# 3rd star number = 13

star_number(5) ➞ 121
# n = 3
# 5th star number = 13
```
### :gem: My Code
```ruby
def star_number(n)
  6 * n * (n-1) + 1
end
```
