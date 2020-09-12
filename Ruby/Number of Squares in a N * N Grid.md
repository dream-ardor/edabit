## Number of Squares in an N * N Grid

Create a function that calculates the number of different squares in an n * n square grid. Check the Resources tab.
```ruby
Examples
number_squares(2) ➞ 5

number_squares(4) ➞ 30

number_squares(5) ➞ 55
```
### :gem: My Code
```ruby
def number_squares(n)
  (1..n).map{|e| e*e}.inject(:+)
end

```
