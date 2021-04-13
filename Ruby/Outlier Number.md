## Outlier Number

Given an array of either entirely odd integers or entirely even integers except for a single Outlier Number. Create a function to return this number.
```ruby
Examples
outlier_number([2, 3, 4]) ➞ 3
# 2 and 4 are even numbers.
# 3 is an outlier number.

outlier_number([1, 2, 3]) ➞ 2

outlier_number([4, 1, 3, 5, 9]) ➞ 4
```
### 💎 My Code
```ruby
def outlier_number(a)
  a.select(&:odd?).size == 1 ? a.select(&:odd?)[0] : a.select(&:even?)[0]
end
```
