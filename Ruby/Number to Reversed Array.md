## Number to Reversed Array

Create a function that takes a number and returns an array with the digits of the number in reverse order.
```ruby
Examples
reverse_arr(1485979) ➞ [9, 7, 9, 5, 8, 4, 1]

reverse_arr(623478) ➞ [8, 7, 4, 3, 2, 6]

reverse_arr(12345) ➞ [5, 4, 3, 2, 1]
```
### :gem: My Code
```ruby
def reverse_arr(n)
  n.to_s.chars.reverse.map(&:to_i)
end
```
