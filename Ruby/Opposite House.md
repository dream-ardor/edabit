## Opposite House 🏘️

Mubashir was walking through a straight street with exactly n identical houses on both sides. House numbers in the street look like this:
```
1 |   | 6

3 |   | 4

5 |   | 2
```
He noticed that Even numbered houses increases on the right while Odd numbered houses decreases on the left.

Create a function that takes a house number house and length of the street n and returns the house number on the opposite side.
```ruby
Examples

opposite_house(1, 3) ➞ 6

opposite_house(2, 3) ➞ 5

opposite_house(3, 5) ➞ 8
```
### :gem: My Code
```ruby
def opposite_house(h,n)
  n * 2 - h + 1
end
```
