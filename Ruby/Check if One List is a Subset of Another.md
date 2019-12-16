## Check if One List is a Subset of Another

List A is contained inside list B if each element in A also exists in B.

The number of times a number is present doesn't matter. In other words, if we transformed both lists into sets, A would be a subset of B.
```ruby
A = [3, 3, 9, 9, 9, 5]
B = [1, 3, 9, 5, 8, 44, 44]

A_Set = [3, 9, 5]
B_Set = [1, 3, 9, 5, 8, 44]

# A_Set is a subset of B_Set
```
Create a function that determines with the first list is a subset of the second.
```ruby
Examples
subset([1, 3], [1, 3, 3, 5]) ➞ True

subset([4, 8, 7], [7, 4, 4, 4, 9, 8]) ➞ True

subset([1, 3], [1, 33]) ➞ False

subset([1, 3, 10], [10, 8, 8, 8]) ➞ False
```
### :gem: My Code
```ruby
subset = lambda a, b: all(x in b for x in a)
```
