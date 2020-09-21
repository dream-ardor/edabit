## Reverse the Number

Create a function that takes an integer n and reverses it.
```python
Examples
rev(5121) ➞ "1215"

rev(69) ➞ "96"

rev(-122157) ➞ "751221"
```
### :snake: My Code
```python
rev = lambda n:str(abs(n))[::-1]
```
