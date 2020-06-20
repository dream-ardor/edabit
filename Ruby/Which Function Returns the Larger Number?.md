## Which Function Returns the Larger Number?

Your function will be passed two functions, f and g, that don't take any parameters. Your function has to call them, and return a string which indicates which function returned the larger number.
```ruby
If f returns the larger number, return the string f.
If g returns the larger number, return the string g.
If the functions return the same number, return the string neither.

Examples
larger(lambda{5}, lambda{10}) ➞ "g"

larger(lambda{25}, lambda{25}) ➞ "neither"

larger(lambda{505050}, lambda{5050}) ➞ "f"

Notes
This exercise is designed as an introduction to higher order functions (functions which use other functions to do their work).
```
### :sunny: My Code
```ruby
def larger(f, g)
  %w[neither f g][f.call <=> g.call]
end
```
