## Skip the Drinks with Too Much Sugar

The function skip_the_sugar() takes in a list of drinks. Make sure the function only returns a list of drinks with no sugar in it or a little bit of sugar.

Drinks that contain too much sugar (in this challenge) are:
```python
Cola
Fanta

Examples
skip_the_sugar(["fanta", "cola", "water"]) ➞ [water]

skip_the_sugar(["fanta", "cola"]) ➞ []

skip_the_sugar(["lemonade", "beer", "water"]) ➞ ["lemonade", "beer", "water"]
```
### :snake: My Code
```python
skip_the_sugar = lambda d:[x for x in d if x not in ['cola','fanta']]
```
