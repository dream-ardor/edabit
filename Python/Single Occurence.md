## Single Occurrence

Create a function that, given a string txt, finds a letter that has a single occurrence. Return the letter in uppercase. If the input is empty, return an empty string "".
```python
Examples
single_occurrence("EFFEAABbc") ➞ "C"

single_occurrence("AAAAVNNNNSS") ➞ "V"

single_occurrence("S") ➞ "S"
```
### :snake: My Code
```python
def single_occurrence(txt):  
  return "".join([i for i in txt.upper() if txt.upper().count(i) == 1])
```
