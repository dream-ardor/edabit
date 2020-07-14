## One, Two, Skip a Few

Create a function which calculates how many numbers are missing from an ordered number line.
```ruby
how_many_missing([1, 2, 3, 8, 9]) ➞ 4

# The number line starts at 1 and ends at 9 (so the numbers 0 and 10 aren't missing from it).
# The numbers missing from this line are 4, 5, 6, and 7.
# 4 numbers are missing.

Examples
how_many_missing([1, 3]) ➞ 1

how_many_missing([7, 10, 11, 12]) ➞ 2

how_many_missing([1, 3, 5, 7, 9, 11]) ➞ 5

how_many_missing([5, 6, 7, 8]) ➞ 0
```
### :gem: My Code
```ruby
def how_many_missing(a)
  a == [] ? 0 : (a[0]..a[-1]).to_a.size - a.size
end
```
