## What Type of Triangle?

Create a function which returns the type of triangle, given the side lengths. Return the following values if they match the criteria.
```ruby
No sides equal: "scalene"
Two sides equal: "isosceles"
All sides equal: "equilateral"

Less or more than 3 sides given: "not a triangle"

Examples
get_triangle_type([2, 6, 5]) ➞ "scalene"

get_triangle_type([4, 4, 7]) ➞ "isosceles"

get_triangle_type([8, 8, 8]) ➞ "equilateral"

get_triangle_type([3, 5, 5, 2]) ➞ "not a triangle"
```
### ⚜️ My Code
```ruby
def get_triangle_type(a)
  a.size == 3 ? ['equilateral', 'isosceles', 'scalene'][(a.uniq).size - 1] : 'not a triangle'
end
```
