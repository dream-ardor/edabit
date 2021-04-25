## Sum Greater Than Five

Write a function that returns the sum of elements greater than 5, in the given array.
```ruby
Examples
sum_five([1, 5, 20, 30, 4, 9, 18]) ➞ 77

sum_five([1, 2, 3, 4]) ➞ 0

sum_five([10, 12, 28, 47, 55, 100]) ➞ 252
```
### 💎 My Code
```ruby
def sum_five(a)
  a.select{|b|b > 5}.reduce(0,:+)
end	
```
