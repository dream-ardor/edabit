## Move Zeroes
Create a function which takes an array arr and moves all zeros to the end, preserving the order of the other elements.
```ruby
Examples
move_zeros([1, 0, 1, 2, 0, 1, 3]) ➞ [1, 1, 2, 1, 3, 0, 0]

move_zeros([0, 1, nil, 2, false, 1, 0]) ➞ [1, nil, 2, false, 1, 0, 0]

move_zeros(['a', 0, 0, 'b', 'c', 'd', 0, 1, 0, 1, 0, 3, 0, 1, 9, 0, 0, 0, 0, 9]) ➞ ['a', 'b', 'c', 'd', 1, 1, 3, 1, 9, 9, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
```
### :gem: My Code
```ruby
def move_zeros(a)
  a.select{|b|b != 0} + a.select{|b|b == 0}
end
```
