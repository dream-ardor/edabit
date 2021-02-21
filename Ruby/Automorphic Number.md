Automorphic Number
A number is called Automorphic number if its square ends in the same digits as the number itself. Create a function that takes a number n and returns true if it is an Automorphic number, otherwise false.
```ruby
Examples
automorphic(1) ➞ true

automorphic(3) ➞ false
# 3^2 = 9

automorphic(6) ➞ true
# 6^2 = 36 (ends with 6)
```
### :gem: My Code
```ruby
def automorphic(n)
  String(n**2).end_with? n.to_s
end
```
