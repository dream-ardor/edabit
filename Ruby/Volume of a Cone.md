## Volume of a Cone

Create a function that takes the height and radius of a cone as arguments and returns the volume of the cone. See the resources tab for the formula.

Volume of a Cone Image
```ruby
Examples
cone_volume(3, 2) ➞ 12.57

cone_volume(15, 6) ➞ 565.49

cone_volume(18, 0) ➞ 0
```
### :gem: My Code
```ruby
def cone_volume(h, r)
 (Math::PI * r**2 * h / 3).round(2)
end
```
