## Lonely Integer

You are given an array of integers having both negative and positive values, except for one integer which can be negative or positive. Create a function to find out that integer.
```ruby
Examples

lonely_integer([1, -1, 2, -2, 3]) ➞ 3
# 3 has no matching negative appearance.

lonely_integer([-3, 1, 2, 3, -1, -4, -2]) ➞ -4
# -4 has no matching positive appearance.

lonely_integer([-9, -105, -9, -9, -9, -9, 105]) ➞ -9
```
### :heart: My Code
```ruby
def lonely_integer(a)
  a.uniq.reduce(:+)
end

#alternate solution
def lonely_integer(a)
  a.select{|b|!a.include?(-b)}[0]
end
```
