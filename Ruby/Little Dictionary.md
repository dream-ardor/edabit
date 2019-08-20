## Little Dictionary
Create a function that takes an initial word and filters out an array to contain words that start with the same letters as the initial word.
```ruby
Examples
dictionary("bu", ["button", "breakfast", "border"]) ➞ ["button"]

dictionary("tri", ["triplet", "tries", "trip", "piano", "tree"]) ➞ ["triplet", "tries", trip"]

dictionary("beau", ["pastry", "delicious", "name", "boring"]) ➞ []
```
### :stars:My Code
```ruby
def dictionary(i, w)
  w.select{|a|a.start_with?(i)}
end
```
