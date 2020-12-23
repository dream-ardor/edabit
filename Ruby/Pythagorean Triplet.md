## Pythagorean Triplet

Create a function that validates whether three given integers form a Pythagorean triplet. The sum of the squares of the two smallest integers must equal the square of the largest number to be validated.
```ruby
Examples
is_triplet(3, 4, 5) ➞ true
# 3² + 4² = 25
# 5² = 25

is_triplet(13, 5, 12) ➞ true
# 5² + 12² = 169
# 13² = 169

is_triplet(1, 2, 3) ➞ false
# 1² + 2² = 5
# 3² = 9
```
### :gem: My Code
```ruby
def is_triplet(*x)
  a, b, c = x.sort
  a ** 2 + b ** 2 == c ** 2
end
```
