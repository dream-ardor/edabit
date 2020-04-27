## The pH Scale

Given a pH value, return whether that value is 'alkaline', 'acidic', or 'neutral'. Return 'invalid' if the value given is less than 0 or greater than 14.
```python
Examples
pH_name(5) ➞ "acidic"

pH_name(8.7) ➞ "alkaline"

pH_name(7) ➞ "neutral"

Notes
Values such as 6.9999 and 7.00001 should return 'acidic' and 'alkaline' respectively.
```
### :computer: My Code
```python
def pH_name(pH):
  if pH < 0 or pH> 14:
    return 'invalid'
  if pH < 7:
    return 'acidic'
  elif pH > 7:
      return 'alkaline'
  else: 
    return 'neutral'
```
