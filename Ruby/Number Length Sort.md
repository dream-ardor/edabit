## Number Length Sort

Create a sorting function which sorts numbers not by numerical order, but by number length! This means sorting numbers with the least digits first, up to the numbers with the most digits.
```ruby
Examples
number_len_sort([1, 54, 1, 2, 463, 2]) ➞ [1, 1, 2, 2, 54, 463]

number_len_sort([999, 421, 22, 990, 32]) ➞ [22, 32, 999, 421, 990]

number_len_sort([9, 8, 7, 6, 5, 4, 31, 2, 1, 3]) ➞ [9, 8, 7, 6, 5, 4, 2, 1, 3, 31]

Notes
If two numbers have the same number of digits, return them in the order they first appeared (this makes it different to just sorting the numbers normally).
```
### :gem: My Code
```ruby
def number_len_sort(a)
  a.sort_by{|b|b.to_s.length}
end
```
