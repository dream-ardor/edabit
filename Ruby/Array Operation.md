## Array Operation

Create a function that takes three parameters and returns an array with the first parameter x, the second parameter y, and every number in between the first and second parameter in ascending order. Then filter through the array and return the array with numbers that are only divisible by the third parameter n.
```ruby
Examples
array_operation(1, 10, 3) ➞ [3, 6, 9]

array_operation(7, 9, 2) ➞ [8]

array_operation(15, 20, 7) ➞ []
```
### :gem: My Code
```ruby
def array_operation(x, y, n)
  (x..y).select{|a| a % n == 0}
end
```
