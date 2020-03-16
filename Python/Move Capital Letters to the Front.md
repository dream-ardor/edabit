## Move Capital Letters to the Front

Create a function that moves all capital letters to the front of a word.
```python
Examples
cap_to_front("hApPy") ➞ "APhpy"

cap_to_front("moveMENT") ➞ "MENTmove"

cap_to_front("shOrtCAKE") ➞ "OCAKEshrt"
```
### :snake: My Code
```python
#regex solution
import re
cap_to_front = lambda s:re.sub('[^A-Z]','',s) + re.sub('[^a-z]','',s)

#join, sorted
def cap_to_front(s):
	return ''.join(sorted(s, key=str.isupper, reverse=True))
  
#list comprehension
def cap_to_front(s):
	return ''.join([c for c in s if c.isupper()]) + ''.join([c for c in s if c.islower()])
```
