## Even and Last
Given an array of integers arr, return the sum of all the integers that have an even index, multiplied by the integer at the last index.

If the sequence is empty, you should return 0.
```ruby
Examples
even_last([2, 3, 4, 5]) ➞ 30
# numbers at even index = 2, 4
# number at last index = 5
# 2*5 + 4*5 = 10 + 20 = 30

even_last([1, 3, 3, 1, 10]) ➞ 140

even_last([]) ➞ 0
```
### 💎 My Code
```ruby
def even_last(a)
  a == [] ? 0 : a.select.with_index { |_, i| i.even? }.reduce(:+) * a[-1] 
end
```
