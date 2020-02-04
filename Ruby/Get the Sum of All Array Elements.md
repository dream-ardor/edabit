## Get the Sum of All Array Elements

Create a function that takes an array and returns the sum of all numbers in the array.
```ruby
Examples
get_sum_of_elements([2, 7, 4]) ➞ 13

get_sum_of_elements([45, 3, 0]) ➞ 48

get_sum_of_elements([-2, 84, 23]) ➞ 105
```
### :gem: My Code
```ruby
def get_sum_of_elements(a)
  a.inject(0,:+)
end
```
