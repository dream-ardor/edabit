## Pyramid Arrays

Given a number n, return an array containing several arrays. Each array increment in size, from range 1 to n inclusive, contaning its length as the elements.
```
Examples
pyramid_arrays(1) ➞ [[1]]

pyramid_arrays(3) ➞ [[1], [2, 2], [3, 3, 3]]

pyramid_arrays(5) ➞ [[1], [2, 2], [3, 3, 3], [4, 4, 4, 4], [5, 5, 5, 5, 5]]
```
### 💎 My Code
```ruby
def pyramid_arrays(n)
  (1..n).map{|a|[a] * a}
end

#alternate
def pyramid_arrays(n)
  (1..n).map{|a| Array.new(a, a)}
end
```
