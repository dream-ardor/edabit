## Next Perfect Square

Mubashir needs your help to find next integral perfect square after the one passed as a parameter.

Create a function which takes a given number n and returns next integral perfect square number. Return nil if the given number is not a perfect square.
```ruby
Examples
next_square(121) ➞ 144

next_square(625) ➞ 676

next_square(114) ➞ nil
# 114 is not a perfect square
```
### 💎 My Code
```ruby
def next_square(n)
  (n ** 0.5 + 1) ** 2 if n ** 0.5 % 1 == 0 
end
```
