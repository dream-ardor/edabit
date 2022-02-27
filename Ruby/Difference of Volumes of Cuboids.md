## Difference of Volumes of Cuboids

Create a program that will take two arrays of integers, a and b. Each array will consist of 3 positive integers, representing the dimensions of cuboids a and b. Find the difference of the cuboids' volumes.

For example, if the parameters passed are ([2, 2, 3], [5, 4, 1]), the volume of a is 12 and the volume of b is 20. Therefore, the function should return 8.
```ruby
Examples
find_difference([ 28, 16, 29 ], [ 7, 8, 17 ]) ➞ 12040

find_difference([ 9, 22, 18 ], [ 16, 24, 10 ]) ➞ 276

find_difference([ 1, 9, 25 ], [ 10, 7, 9 ]) ➞ 405

find_difference([ 7, 6, 16 ], [ 26, 9, 26 ]) ➞ 5412
```
### 💎  My Code
```ruby
def find_difference(a, b)
  (a.reduce(:*) - b.reduce(:*)).abs
end
```
