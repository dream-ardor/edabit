## Taxi Journey
A taxi journey costs $3 for the first kilometer travelled. However, all kilometers travelled after that will cost $2 each.

Create a function which returns the distance that the taxi must've travelled, given the cost as a parameter.
```ruby
Examples
journey_distance(3) ➞ 1
# The first kilometer costs $3

journey_distance(9) ➞ 4
# The first kilometer costs $3 plus the other three kilometers (costing $2 each)

journey_distance(5) ➞ 2
```

### :gem: My Code
```ruby
def journey_distance(n)
  n/2.floor #or n/2.ceil
end
```
