## Online Shopping

Create a function that determines whether a shopping order is eligible for free shipping. An order is eligible for free shipping if the total cost of items purchased exceeds $50.00.
```ruby
Examples
free_shipping({ "Shampoo": 5.99, "Rubber Ducks": 15.99 }) ➞ False

free_shipping({ "Flatscreen TV": 399.99 }) ➞ True

free_shipping({ "Monopoly": 11.99, "Secret Hitler": 35.99, "Bananagrams": 13.99 }) ➞ True
```

### :maple_leaf: My Code
```ruby
def free_shipping(o):
  return sum(o.values()) > 50
```
