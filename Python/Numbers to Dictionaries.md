## Numbers to Dictionaries

Mubashir needs your help in a simple task.

Given a list of numbers lst:
```
Create a dictionary for each given number.
The dictionary key will be the number converted string.
The value will be the corresponding character code converted string (check ASCII table).
Return a list of the resulting dictionaries.

Examples

num_to_dict([118, 117, 120]) ➞ [{"118":"v"}, {"117":"u"}, {"120":"x"}]

num_to_dict([101, 121, 110, 113, 103]) ➞ [{"101":"e"}, {"121":"y"}, {"110":"n"}, {"113":"q"}, {"103":"g"}]

num_to_dict([118, 103, 110]) ➞ [{"118":"v"}, {"103":"g"}, {"110":"n"}]
```
### 🐍 My Code
```python
num_to_dict = lambda l:[{str(i):chr(i)} for i in l]
```
