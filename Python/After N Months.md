## After N Months...

Create a function that takes in year and month as input, then return what year it would be after n-months has elapsed.
```python
Examples
after_n_months(2020, 24) ➞ 2022

after_n_months(1832, 2) ➞ 1832

after_n_months(1444, 60) ➞ 1449

Notes:
Assume that adding 12 months will always increment the year by 1.
If no value is given for year or months, return "year missing" or "month missing".
```
### :snake: My Code
```python
def after_n_months(y, m):
  if not m:return 'month missing'
  if not y:return 'year missing'
  else:return round(m/12 + y)
```
