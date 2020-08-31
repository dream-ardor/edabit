## Find the Bomb

Create a function that finds the word "bomb" in the given string. If found, return "Duck!!!", otherwise, return "There is no bomb, relax.".
```ruby
Examples
bomb("There is a bomb.") ➞ "Duck!!!"

bomb("Hey, did you think there is a bomb?") ➞ "Duck!!!"

bomb("This goes boom!!!") ➞ "There is no bomb, relax."

Notes
"bomb" may appear in different cases (i.e. uppercase, lowercase, mixed).
```
### :bomb: My Code
```ruby
def bomb(t)
 t =~ /bomb/i ? "Duck!!!" : "There is no bomb, relax."
end
```
