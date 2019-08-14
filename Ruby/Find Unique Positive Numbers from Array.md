## Find Unique Positive Numbers from Array
Write a function that takes an array and returns a new array with unique positive (more than 0) numbers.
```ruby
Examples
unique_arr([-5, 1, -7, -5, -2, 3, 3, -5, -1, -1]) ➞ [1, 3]

unique_arr([3, -3, -3, 5, 5, -6, -2, -4, -1, 3]) ➞ [3, 5]

unique_arr([10, 6, -12, 13, 5, 5, 13, 6, 5]) ➞ [10, 6, 13, 5]
```
### :rocket:My Code
```ruby
def unique_arr(arr)
  arr.select{|x | x > 0}.uniq
end
```
