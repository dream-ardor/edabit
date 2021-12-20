## Maximum Weight Allowed

Creat a function that returns true if the combined weight of a car car and the weight of the passengers p in the car is less than the maximum weight max_weight the car is allowed to carry. Otherwise, return false. The weight of the car and the weight of the passengers are given in pounds. The maximum weight is given in kilograms.
```
Examples
weight_allowed(3000, [150, 201, 75, 88, 195], 1700) ➞ true

weight_allowed(3200, [220, 101, 115, 228, 15], 1700) ➞ false

weight_allowed(2900, [225, 171, 300, 274, 191], 1850) ➞ true
```
### 💎 My Code
```ruby
def weight_allowed(c, p, m)
  c + p.inject(:+) < m * 2.2
end
```
