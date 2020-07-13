## Same Parity?

Create a function that takes a number as input and returns true if the sum of its digits has the same parity as the entire number. Otherwise, return false.
```ruby
Examples
parity_analysis(243) ➞ true
# 243 is odd and so is 9 (2 + 4 + 3)

parity_analysis(12) ➞ false
# 12 is even but 3 is odd (1 + 2)

parity_analysis(3) ➞ true
# 3 is odd and 3 is odd and 3 is odd (3)

Notes:
Parity is whether a number is even or odd. If the sum of the digits is even and the number itself is even, return true. The same goes if the number is odd and so is the sum of its digits.
Single digits will obviously have the same parities (see example #3).
```
### My Code
```ruby
def parity_analysis(num)
  num % 2 == num.to_s.chars.map(&:to_i).inject(:+) % 2
end

#alternate
def parity_analysis(n)
  n.to_s.chars.map(&:to_i).inject(:+).odd? && n.odd? ||
  n.to_s.chars.map(&:to_i).inject(:+).even? && n.even?
end
```
