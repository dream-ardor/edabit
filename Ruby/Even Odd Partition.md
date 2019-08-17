## Even Odd Partition
Write a function that partitions the array into two subarrays: one with all even integers, and the other with all odd integers. Return your result in the following format:

[[evens], [odds]]
```ruby
Examples
even_odd_partition([5, 8, 9, 2, 0]) ➞ [[8, 2, 0], [5, 9]]

even_odd_partition([1, 0, 1, 0, 1, 0]) ➞ [[0, 0, 0], [1, 1, 1]]

even_odd_partition([1, 3, 5, 7, 9]) ➞ [[], [1, 3, 5, 7, 9]]

even_odd_partition([]) ➞ [[], []]
```
### :gem: My Code
```ruby
def even_odd_partition(arr)
  arr.partition{|x| x.even?}
end
```
