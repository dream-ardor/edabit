## Zip It, If You Can?

Given a list of women and a list of men, either:

Return "sizes don't match" if the two lists have different sizes.
If the sizes match, return a list of pairs, with the first woman paired with the first man, second woman paired with the second man, etc.
```python
Examples
zip_it(['Elise', 'Mary'], ['John', 'Rick']) 
 ➞ [('Elise', 'John'), ('Mary', 'Rick')]

zip_it(['Ana', 'Amy', 'Lisa'], ['Bob', 'Josh']) 
 ➞ "sizes don't match"

zip_it(['Ana', 'Amy', 'Lisa'], ['Bob', 'Josh', 'Tim'])
 ➞ [('Ana', 'Bob'), ('Amy', 'Josh'), ('Lisa', 'Tim')]
 ```
 ### :snake: My Code
 ```python
 def zip_it(a, b):
  return list(zip(a,b)) if len(a)==len(b) else "sizes don't match"
 ```
