## Grab the City

Write a function to return the city from each of these vacation spots.
```python
Examples
grab_city("[Last Day!] Beer Festival [Munich]") ➞ "Munich"

grab_city("Cheese Factory Tour [Portland]") ➞ "Portland"

grab_city("[50% Off!][Group Tours Included] 5-Day Trip to Onsen [Kyoto]")
```
### :snake: My Code
```python
def grab_city(t):
  return t.split('[')[-1][:-1]
```
