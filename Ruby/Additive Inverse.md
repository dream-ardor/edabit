## Additive Inverse

A number added with its additive inverse equals zero. Create a function that returns an array of additive inverses.
```ruby
Examples
additive_inverse([5, -7, 8, 3]) ➞ [-5, 7, -8, -3]

additive_inverse([1, 1, 1, 1, 1]) ➞ [-1, -1, -1, -1, -1]

additive_inverse([-5, -25, 35]) ➞ [5, 25, -35]
```
### :gem: My Code
```ruby
def additive_inverse(a)
 a.map(&:-@)
end
```
