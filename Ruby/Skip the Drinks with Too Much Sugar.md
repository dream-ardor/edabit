## Skip the Drinks with Too Much Sugar

The function skip_the_sugar() takes in an array of drinks. Make sure the function only returns an array of drinks with no sugar in it or a little bit of sugar.

Drinks that contain too much sugar (in this challenge) are:
```
Cola
Fanta
```
```ruby
Examples
skip_the_sugar(["fanta", "cola", "water"]) ➞ [water]

skip_the_sugar(["fanta", "cola"]) ➞ []

skip_the_sugar(["lemonade", "beer", "water"]) ➞ ["lemonade", "beer", "water"]
```
### :gem: My Code
```ruby
def skip_the_sugar(d)
  d -=['cola', 'fanta']
end
```
