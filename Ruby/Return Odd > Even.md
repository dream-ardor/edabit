## Return Odd > Even
Given an array, return true if there are more odd numbers than even numbers, otherwise return false.
```ruby
Examples
odd_even([1, 2, 3, 4, 5, 6, 7, 8, 9]) ➞ true

odd_even([1]) ➞ true

odd_even([13452394823795273847528572346]) ➞ false
```
### :gem: My Code
```ruby
def odd_even(a)
 a.count(&:odd?) > a.count(&:even?)
end
```
