## Circle or Square

Given the radius of a circle and the area of a square, return true if the circumference of the circle is greater than the square's perimeter and false if the square's perimeter is greater than the circumference of the circle.
```ruby
Examples
circle_or_square(16, 625) ➞ true

circle_or_square(5, 100) ➞ false

circle_or_square(8, 144) ➞ true
```
### 💎 My Code
```ruby
def circle_or_square(r,a)
  r * 1.57 > a ** 0.5
end
```
