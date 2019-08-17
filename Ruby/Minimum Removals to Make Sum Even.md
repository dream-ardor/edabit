## Minimum Removals to Make Sum Even
Create a function that returns the minimum number of removals to make the sum of all elements in an array even.
```ruby
Examples
minimum_removals([1, 2, 3, 4, 5]) ➞ 1

minimum_removals([5, 7, 9, 11]) ➞ 0

minimum_removals([5, 7, 9, 12]) ➞ 1
```

### :gem: My Code
```ruby
def minimum_removals(arr)
  arr.reduce(:+).even? ? 0 : 1
end
```
