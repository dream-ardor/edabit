## Sum of Cubes
Create a function that takes an array of numbers and returns the sum of its cubes.
```ruby
Examples
sum_of_cubes([1, 5, 9]) ➞ 855
# Since 1^3 + 5^3 + 9^3 = 1 + 125 + 729 = 855

sum_of_cubes([3, 4, 5]) ➞ 216

sum_of_cubes([2]) ➞ 8

sum_of_cubes([]) ➞ 0
```
### :trident: My Code
```ruby
def sum_of_cubes(n)
  n.reduce(0){|x,y| x+y ** 3}
end
```
