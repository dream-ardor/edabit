## Maximum Possible Total

Given an array of 10 numbers, return the maximum possible total made by summing just 5 of the 10 numbers.
```ruby
Examples
max_total([1, 1, 0, 1, 3, 10, 10, 10, 10, 1]) ➞ 43

max_total([0, 0, 0, 0, 0, 0, 0, 0, 0, 100]) ➞ 100

max_total([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]) ➞ 40
```
### :gem: My Code
```ruby
def max_total(n)
  n.sort.last(5).inject(:+)
end
```
