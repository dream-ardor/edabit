## Adding Numbers in a String

Given a string of numbers separated by a comma and space, return the total of all the numbers.
```ruby
Examples
add_nums("2, 5, 1, 8, 4") ➞ 20

add_nums("1, 2, 3, 4, 5, 6, 7") ➞ 28

add_nums("10") ➞ 10
```
### :computer: My Code
```ruby
def add_nums(n)
  n.split(',').map(&:to_i).inject(:+)
end
```
