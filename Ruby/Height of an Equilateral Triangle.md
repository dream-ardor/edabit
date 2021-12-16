## Height of an Equilateral Triangle

Create a function that takes the length of the side of an equilateral triangle in centimeters and returns the height of the triangle in millimeters.
```
Examples
height(2) ➞ 17.3 mm

height(5) ➞ 43.3 mm

height(6.2) ➞ 53.7 mm
```
### 💎 My Code
```ruby
def height(s)
  "#{(8.66 * s).round(1)} mm"
end
```
