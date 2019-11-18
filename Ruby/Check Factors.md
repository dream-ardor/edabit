## Check Factors
Write a function that returns true if all integers in an array are factors of a number, and false otherwise.
```ruby
Examples
check_factors([2, 3, 4], 12) ➞ true
# Since 2, 3, and 4 are all factors of 12.

check_factors([1, 2, 3, 8], 12) ➞ false
# 8 is not a factor of 12.

check_factors([1, 2, 50], 100) ➞ true

check_factors([3, 6], 9) ➞ false
```
### :gem: My Code
```ruby
def check_factors(f, n)
  f.all?{|x|n % x == 0}
end
```
