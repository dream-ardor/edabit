## Give Me the Even Numbers

Create a function that takes two parameters (start, stop), and returns the sum of all even numbers in the range.
```ruby
Examples
sum_even_nums_in_range(10, 20) ➞ 90
# 10, 12, 14, 16, 18, 20

sum_even_nums_in_range(51, 150) ➞ 5050

sum_even_nums_in_range(63, 97) ➞ 1360

Notes
Remember that the start and stop values are inclusive.
```
### :computer: My Code
```ruby
def sum_even_nums_in_range(a,b)
  (a..b).select(&:even?).reduce(:+)
end
```
