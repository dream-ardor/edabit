## Multiply by Length
Create a function to multiply all values in an array by the amount of values in that array.
```ruby
Examples
multiply_by_length([2, 3, 1, 0]) ➞ [8, 12, 4, 0]

multiply_by_length([4, 1, 1]) ➞ ([12, 3, 3])

multiply_by_length([1, 0, 3, 3, 7, 2, 1]) ➞  [7, 0, 21, 21, 49, 14, 7]

multiply_by_length([0]) ➞ ([0])
```
### :rocket:My Code
```ruby
def multiply_by_length(arr)
  arr.map{|x| x * arr.length}
end
```
