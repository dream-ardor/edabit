## Rotate Max Number

Create a function that takes a number and returns the maximum value by rearranging its digits.
```ruby
Examples
rotate_max_number(123) ➞ 321

rotate_max_number("001") ➞ 100

rotate_max_number(999) ➞ 999
```
### :gem: My Code
```ruby
def rotate_max_number(n)
  n.to_s.chars.sort.reverse.join.to_i
end
```
