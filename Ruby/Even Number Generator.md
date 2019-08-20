## Even Number Generator
Create a function that finds all even numbers from 1 to the given number.
```ruby
Examples
find_even_nums(8) ➞ [2, 4, 6, 8]

find_even_nums(4) ➞ [2, 4]

find_even_nums(2) ➞ [2]
```
### :stars: My Code
```ruby
def find_even_nums(n)
  (2..n).select(&:even?)
end
```
