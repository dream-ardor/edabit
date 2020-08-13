## Summing a Slice

Given an array and an integer n, return the sum of the first n numbers in the array.
```ruby
Examples
slice_sum([1, 3, 2], 2) ➞ 4

slice_sum([4, 2, 5, 7], 4) ➞ 18

slice_sum([3, 6, 2], 0) ➞ 0

Notes:
If n is larger than the length of the array, return the sum of the whole array.
```
### :gem: My Code
```ruby
def slice_sum(a, n)
  a.first(n).reduce(0, :+)
end
```
