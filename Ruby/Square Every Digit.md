## Square Every Digit

Create a function that squares every digit of a number.
```ruby
Examples
square_digits(9119) ➞ 811181

square_digits(2483) ➞ 416649

square_digits(3212) ➞ 9414
```
### :computer: My Code
```ruby
def square_digits(n)
  n.to_s.chars.map{|d| d.to_i ** 2}.join.to_i
end
```
